---
title: Domande frequenti
description: Trova le risposte alle domande frequenti su OpenPBR e Substance 3D.
source-git-commit: a3ceb4df30f08099799bc2caecc5446d3832fc06
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---


# Domande frequenti su OpenPBR

## Il modello di OpenPBR

+++Che cos’è OpenPBR e quale versione supporta Painter?

OpenPBR è una specifica di materiale aperto ospitata da Academy Software Foundation, che definisce un modello di ombreggiatura standardizzato progettato per funzionare in modo coerente tra le applicazioni. [Nella documentazione di Painter sono disponibili ulteriori informazioni sull&#39;utilizzo di OpenPBR](https://experienceleague.adobe.com/it/docs/substance-3d-painter/using/home).

+++

+++Cosa significa quando un&#39;applicazione dichiara di &quot;supportare l&#39;OpenPBR&quot; e come è possibile scoprire in che modo è supportato da un&#39;applicazione specifica?

Non esiste un processo di certificazione formale, quindi l&#39;attestazione può significare cose diverse. In pratica, le implementazioni variano: alcune coprono l&#39;intera specifica, altre solo un sottoinsieme, lasciando fuori funzioni come la pellicola sottile, la dispersione, o certi comportamenti subsuperficiali. Si noti inoltre che &quot;Supporto MaterialX&quot; e &quot;Supporto OpenPBR&quot; non sono la stessa cosa; un&#39;applicazione può supportare uno senza implementare completamente l&#39;altro.

Per scoprire cosa supporta realmente un&#39;applicazione specifica, utilizzate una combinazione di approcci: controllate le note di rilascio (il supporto viene spesso aggiunto in modo incrementale); caricate l&#39;OpenPBR Playground dell&#39;ASWF e confrontatelo rapidamente con un rendering di riferimento per le aperture; o per gli studi con investimenti significativi nella pipeline, chiedete direttamente al fornitore le funzionalità supportate e la relativa roadmap.

+++

+++È possibile garantire risultati identici in applicazioni e moduli di rendering diversi?

Non del tutto, e questo è progettato. L’OpenPBR definisce un modello di materiale condiviso, ma anche l’aspetto finale viene modellato in base all’illuminazione, agli algoritmi di rendering, alla gestione del colore e alla precisione con cui ogni implementazione è conforme alle specifiche.

In pratica, massimizzare questa garanzia significa: esportare tramite USD con l&#39;integrazione di MaterialX; convalidare il round-trip in anticipo utilizzando l&#39;OpenPBR Shader Playground dell&#39;ASWF piuttosto che alla fine della produzione; confermare i livelli di supporto dei fornitori per qualsiasi funzione avanzata utilizzata; e accordarsi in anticipo su quali funzionalità verranno utilizzate e non verranno utilizzate nei materiali condivisi. La portabilità deve essere attivamente convalidata, non presunta.

+++

+++Esistono materiali che OpenPBR non è in grado di rappresentare accuratamente?

Sì. OpenPBR è un modello parametrico. Parametri come rugosità, metallizzazione e IOR coprono la maggior parte dei casi d&#39;uso di produzione, ma non possono replicare la precisione dei formati di materiale misurati come X-Rite AxF, che acquisiscono i dati ottici effettivi da un campione fisico. Per un lavoro di produzione generale, l&#39;OpenPBR è adatto; per le applicazioni che richiedono una corrispondenza esatta del campione, un formato misurato può essere più appropriato.

La pittura dell&#39;automobile è un&#39;illustrazione utile. È possibile creare pittura auto in OpenPBR con un paio di avvertenze. L&#39;OpenPBR non include uno shader per pitture per auto specializzato, quindi potrebbe essere insufficiente per alcuni usi dell&#39;industria automobilistica. Inoltre, dipende semplicemente dal tipo di pittura dell&#39;auto — alcune pitture dell&#39;auto avranno sempre proprietà che non rientrano nell&#39;ambito di applicazione di qualsiasi dato shader. Ma tenendo presenti questi punti, la pittura dell&#39;auto si mappa naturalmente sull&#39;architettura a strati di OpenPBR.

+++

## Impostazione e conversione

+++Devo imparare OpenUSD o MaterialX per usare OpenPBR?

No. Per la maggior parte degli artisti, l&#39;OpenPBR è semplicemente il modello di materiale integrato negli strumenti che già usano. Substance 3D Painter, Maya 2025.3 e 3ds Max 2026 utilizzano tutti l’OpenPBR come materiale predefinito; lavorare con esso significa solo lavorare con lo shader standard. USD e MaterialX diventano rilevanti solo quando i materiali devono spostarsi tra le applicazioni. Per i flussi di lavoro a singola applicazione, il supporto nativo è sufficiente; per le pipeline multi-DCC, USD e MaterialX forniscono l&#39;infrastruttura di interscambio, ma in gran parte in background.

Detto questo, il percorso di scambio più efficace per le librerie di materiali condivise avviene tramite USD con integrazione MaterialX, che fornisce un contenitore standardizzato indipendente dal rendering per le descrizioni dei materiali. I flussi di lavoro per l&#39;esportazione di materiali come risorse autonome (senza un modello associato, da utilizzare in una libreria condivisa) sono ancora in fase di sviluppo attivo e non sono ancora completamente supportati ovunque. Prima di eseguire il commit in un&#39;architettura di libreria che dipende da questo, convalidare la pipeline specifica in base alle funzionalità correnti.

+++

+++Come si crea un nuovo progetto di OpenPBR in Substance 3D Painter?

Per impostazione predefinita, nei progetti privi di modello viene utilizzato lo shader OpenPBR. L&#39;OpenPBR è ora la prima opzione nella finestra del nuovo progetto e sostituisce ASM. Sono inoltre disponibili modelli dedicati per flussi di lavoro specifici (Anisotropia, Pelo, Fuzz, Dispersione sottosuperficie) e l’importazione di un file USD contenente materiale di OpenPBR consente di configurare automaticamente il progetto. Anche i progetti di esempio forniti con Substance 3D Painter sono stati aggiornati in modo da utilizzare il flusso di lavoro di OpenPBR e rappresentano un buon punto di partenza per familiarizzare con il funzionamento pratico.

+++

+++È possibile convertire in OpenPBR un progetto di Adobe Standard Material (ASM) esistente?

Nessuna conversione automatica. I progetti ASM esistenti mantengono lo shader corrente quando vengono aperti e i modelli ASM rimangono disponibili per i nuovi progetti.

Per eseguire manualmente la migrazione all’OpenPBR, seleziona lo shader nella finestra delle impostazioni dello Shader, quindi aggiungi i relativi canali di OpenPBR tramite le impostazioni del set di texture > Aggiungi o rimuovi canali. Al termine, rivedi i livelli esistenti per assicurarti che il loro contenuto sia destinato ai canali desiderati.

+++

+++È necessario aggiornare gli shader personalizzati per OpenPBR?

No: gli shader personalizzati esistenti continuano a funzionare, poiché le librerie di shader pertinenti sono obsolete anziché rimosse. Tuttavia, si consiglia di eseguire la migrazione alle nuove librerie di shader, in modo che siano più pulite e facili da utilizzare. Per ulteriori informazioni, consultate il registro delle modifiche dell’API shader nel menu Aiuto.

+++

## Utilizzo in-app

+++Con così tanti parametri disponibili in OpenPBR, dove devo concentrare la mia attenzione?

Inizia con la semplicità. Per la maggior parte delle superfici opache, Colore di base, rugosità Specular e metallizzazione rappresentano la maggior parte delle differenze visibili tra i materiali. Aggiungi IOR se la riflettività è importante; perfeziona il colore dello Specular se il materiale ha una tinta con angolo di pascolo. Abilita la trasmissione, il sottosuolo, il rivestimento, il fuzz, i film sottili e la dispersione solo quando hai una ragione chiara e basata sui riferimenti per farlo, dal momento che ogni canale aggiuntivo aggiunge complessità e potenziale costo di rendering. Nascondere o comprimere i gruppi di parametri inutilizzati mantiene l’area di lavoro concentrata e riduce il rischio di effetti indesiderati.

+++

+++Ho una mappa della rugosità: devo collegarla alla rugosità della Diffusa di base o alla rugosità degli Specular?

Rugosità Specular: controlla la nitidezza del riflesso ed è l’equivalente diretto della rugosità immessa in altri flussi di lavoro PBR. La rugosità di base della Diffusa è un parametro separato e specializzato che influisce solo sulla dispersione diffusa; per la maggior parte dei flussi di lavoro può rimanere al suo valore predefinito.

+++

+++Perché cambiare Colore di base non ha alcun effetto quando si utilizza la dispersione sottosuperficiale?

Esiste una &quot;gerarchia di priorità&quot; che determina l&#39;influenza di ciascun parametro sull&#39;aspetto finale del materiale. Metti Mi piace così:

* Metalness viene prima: quando Metalness=1, le parti Subsurface e Transmission vengono disattivate.
* Il successivo passo successivo è il peso di trasmissione: se il peso di trasmissione è pari a 1, la sottosuperficie sarà assente.
* Spessore sottosuperficie viene dopo questo.
* Il Colore di base di Diffuse viene per ultimo: la diffusione di base contribuisce solo quando nessuna delle precedenti impostazioni è impostata su 1.

Quindi, nell&#39;esempio indicato, se Spessore sottosuperficie è impostato su 1 (il suo valore massimo), allora governa tutto l&#39;aspetto. La modifica del valore Colore di base non ha alcun effetto perché la Diffusa Base non apporta alcun contributo. Al contrario, se Metalness è impostato sul valore massimo di 1, la modifica dei valori di Spessore trasmissione, Spessore sottosuperficie e Colore di base di Diffusa non avrà alcun effetto sull’aspetto finale del materiale. Trasmissione, Sottosuperficie e Diffusa sono tutti dielettrici (non metallici), quindi l&#39;impostazione di Metalness su 1 rimuove qualsiasi contributo non metallico.

+++

+++Perché la trasmissione si comporta in modo imprevisto? Ad esempio, perché la trama appare molto scura quando la attivi?

Il colpevole più frequente è che la Profondità di trasmissione è troppo bassa. Questo parametro definisce quanto si sposta la luce prima che il colore di trasmissione raggiunga la saturazione completa; a valori bassi, anche la geometria sottile appare scura e densa. Aumentalo per adattarlo alla scala fisica approssimativa dell&#39;oggetto. Se il materiale appare troppo chiaro, regolate il Colore di trasmissione e Profondità insieme per trovare il giusto bilanciamento.

La dispersione può aggiungere un ulteriore livello di complessità. Il colore di trasmissione non è una tinta semplice: il suo effetto dipende da quanto la luce viaggia attraverso l&#39;oggetto, controllata dalla Profondità di trasmissione. Colore dispersione, nel frattempo, controlla un percorso separato che la luce può intraprendere, rimbalzando all&#39;interno del materiale invece di passare direttamente attraverso. Poiché la dispersione è direzionale, anche il risultato cambia a seconda di dove viene posizionata la sorgente luminosa. Regolarne una senza considerare l&#39;altra è una fonte comune di risultati imprevisti.

+++

+++Ho attivato Thin-film ma non riesco a vedere alcun effetto. Cosa mi manca?

Controlla prima il valore Thickness. In modo controintuitivo, valori più sottili producono una iridescenza più visibile; la maggior parte degli effetti si verifica tra 0 e 1 micrometro. Se l’effetto è ancora debole, regolate lo IOR in modo da spostare sia l’intensità che il colore dell’interferenza. Conferma inoltre che il peso della pellicola sottile è superiore a zero.

+++
