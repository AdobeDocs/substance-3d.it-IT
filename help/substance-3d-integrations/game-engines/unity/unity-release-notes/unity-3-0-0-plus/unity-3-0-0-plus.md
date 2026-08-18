---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-3-0-0-plus.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 3.0.0 e successive per scoprire le nuove funzioni e i miglioramenti.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# Unità 3.0.0+

## Unità 3.12.0

<b>Aggiunto/Aggiornato:</b>

* Supporto per Substance 3D Connector in Unity, con funzionalità SendTo per l’invio di risorse tra Substance 3D Sampler e Unity.
* Supporto per la ridenominazione e la ripubblicazione di grafici .sbsar da Designer a Unity, assicurando che le modifiche apportate in Designer persistano quando il grafico aggiornato viene reimportato nel plug-in Unity.
* Documentazione per la condivisione di file .sbsar tra progetti Unity.
* Pagina del contributo della community alla documentazione del plug-in Unity: https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/community-contributions.html.

<b>Corretto:</b>

* Problema a causa del quale la miniatura del materiale nella cartella Risorse progetto unità non viene aggiornata dopo la ripubblicazione di un file .sbsar, visualizzando il materiale precedente anziché quello corrente.

## Unità 3.11.0

<b>Aggiunto/Aggiornato:</b>

* Sono state migliorate le prestazioni per i progetti con oltre 1000 grafici Substance, riducendo in modo significativo i tempi di risposta dell’interfaccia utente durante l’ispezione dei file sbsar nella cartella Assets.
* È stato aggiunto un pulsante di ripristino per ripristinare i file sbsar allo stato originale, migliorando l’efficienza del flusso di lavoro.
* Documentazione aggiornata con una soluzione alternativa al problema &quot;Input di immagini bloccati a 8 bit&quot;, disponibile all&#39;indirizzo: [Integrazioni di Substance 3D in Unity - Aggiornamento di progetti e problemi noti](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).
* Documentazione aggiornata per risolvere l&#39;errore &quot;Asserzione non riuscita sull&#39;espressione&quot; rilevato durante la navigazione nelle cartelle del pannello in Unity: [Integrazioni Substance 3D in Unity - Aggiornamento di progetti e problemi noti](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).

<b>Corretto:</b>

* È stato risolto un problema che causava l’interruzione del plug-in sulle piattaforme Linux.
* Sono stati risolti problemi di compatibilità con il plug-in Unity nella versione 2023.

## Unità 3.10.1

<b>Corretto:</b>

* È stato risolto un problema che impediva il caricamento della Substance Engine a causa di un problema con sbsario.dll nel plug-in Substance 3D for Unity.

## Unità 3.10.0

<b>Aggiunto/Aggiornato:</b>

* È stata aggiornata la sezione dei commenti per l’API RenderInstanceAsync nel plug-in.

<b>Corretto:</b>

* È stato risolto un problema di perdita di memoria nel codice C++ del plug-in, garantendo il recupero completo della memoria al momento dello smaltimento degli oggetti.
* È stato risolto un problema in Linux a causa del quale l’importazione del pacchetto di plug-in Unity provocava un errore &quot;SubstanceException: è stato fornito un argomento non valido all’API&quot;, consentendo ora l’importazione corretta dei file SBSAR.
* È stato risolto un problema a causa del quale SubstanceGraphSO.CurrentStatePreset non funzionava correttamente per il caricamento dei predefiniti con uno script della finestra dell’editor personalizzato in Unity. Uno script correttivo è ora disponibile nella pagina della documentazione Substance (HelpX): https://experienceleague.adobe.com/en/docs/substance-3d/ecosystem/game-engines/unity/substance-3d-for-unity-scripting/substance-3d-for-unity-scripting
* È stato corretto un bug a causa del quale le proprietà del grafico scomparivano dopo la riselezione nell’editor Unità.
* È stato risolto il problema &quot;Tipo gestito sconosciuto a cui si fa riferimento&quot; relativo a SubstanceGraphSO nel plug-in Unity, migliorando la compatibilità e la funzionalità sulle piattaforme Android, in particolare per Unity 2022.1 e potenzialmente in tutte le versioni di Unity.
* È stato risolto un problema a causa del quale la selezione &quot;FORMATO NORMALE&quot; nella sezione PARAMETRI TECNICI veniva visualizzata in modo errato come campo di input numerico, anziché come elenco a discesa previsto con le opzioni DirectX e OpenGL.

## Unità 3.9.0

<b>Aggiunto/Aggiornato:</b>

* I file Sbsar ora possono essere trascinati e rilasciati nel progetto. L&#39;oggetto .sbsar può essere applicato a una trama come previsto in Unity 2022.3.
* Documentazione avanzata per il plug-in.

<b>Corretto:</b>

* È stato risolto un problema a causa del quale il plug-in Unity non funzionava su Android.
* Vincoli di denominazione risolti nel plug-in Unity. Quando un nome di file conteneva un &quot;.&quot;, il plug-in non caricava correttamente il file.
* È stato risolto un problema a causa del quale, deselezionando &quot;Genera tutti gli output&quot;, la texture in eccesso non veniva eliminata automaticamente.
* È stata corretta l’importazione errata di materiali SBSAR nei progetti standard Unity 2021.3. Ora, nel progetto del modello standard, i materiali SBSAR possono essere importati nella cartella delle risorse e applicati a una trama 3D senza errori.
* È stata corretta l’importazione errata di materiali SBSAR nei progetti HDRP Unity 2021/2022. Ora, nel progetto del modello HDRP, i materiali SBSAR possono essere importati nella cartella delle risorse e applicati a una trama 3D senza errori.
* È stato corretto un errore di compilazione durante la generazione della build Android per produrre l’APK: &quot;Compilazione non riuscita. Per informazioni dettagliate, vedere l’output degli errori del compilatore.&quot;
* È stato risolto un problema che causava un errore del processo di creazione del progetto con errori in Windows.
* È stato risolto un problema che causava un errore nel processo di creazione del progetto su Android: UnityEditor.BuildPlayerWindow+BuildMethodException.
* È stata risolta l&#39;eccezione UnityException rilevata durante la modifica degli input di SubstanceGraph in fase di runtime. In precedenza, richiamando SubstanceRuntimeGraph.SetTexturesResolution e SubstanceRuntimeGraph.Render(), SubstanceGraph ha generato il rendering di risultati errati.
* È stato corretto un errore tipografico in SubstanceEditorTools.cs.

## Unità 3.8.0

<b>Aggiunto/Aggiornato:</b>

* È stato introdotto il supporto per i parametri con visibilità condizionale (funzione Visible If).
* Aggiornamento del motore di Substance alla versione 9.
* Documentazione aggiornata per risolvere un problema relativo a NativeGraph.InRenderWork che non funziona in uno script della finestra dell&#39;editor personalizzato. Ulteriori dettagli sono disponibili qui: [Substance 3D for Unity Scripting - Class Documentation](../../../../game-engines/unity/3d-for-unity-scripting/class-documentation/substanceruntime-class/substanceruntime-class.md)

<b>Corretto:</b>

* È stato risolto un problema che interessava le mappe normali nei progetti Android.
* È stato risolto un bug a causa del quale, trascinando inavvertitamente un oggetto sbsar nella vista della scena, tutti gli oggetti spostati venivano sostituiti dal materiale dell’oggetto sbsar.
* È stato corretto un bug che causava un errore durante l’ispezione di un materiale contrassegnato come Solo runtime in modalità Runtime e l’apertura della mappatura della texture di output.

## Unità 3.7.0

<b>Aggiunto/Aggiornato:</b>

* Supporto per predefiniti incorporati ed esterni
* Compatibilità con Unity 2022.2

<b>Corretto:</b>

* Errore durante la creazione di un nuovo grafico per un file sbsar utilizzando il pulsante Copia grafico: &quot;Trasferimento ricorsivo imprevisto della classe con script&quot;
* Creazione di cartelle di materiale aggiuntivo su Mac dopo la riapertura di un progetto
* La matrice SubstanceFileSO non si aggiorna durante la creazione o l&#39;eliminazione di istanze del grafico
* Visualizzazione di opzioni di input errate durante la duplicazione di una Substance
* Campi etichetta vuoti nelle esportazioni di file .sbsprs
* Errori durante l&#39;esportazione/importazione predefinita nell&#39;editor: EndLayoutGroup: BeginLayoutGroup deve essere chiamato per primo.

<b>Rimosso:</b>

* Sezione Canali dal plug-in Unity a causa della mancanza di valore utente

## Unità 3.6.0

<b>Aggiunto/Aggiornato:</b>

* Possibilità di rendere modificabili in modo indipendente i singoli valori Int 4.

<b>Corretto:</b>

* Problema a causa del quale, alla riapertura di un progetto, i materiali tornavano a uno stato precedente
* Errore durante la modifica del grafico del materiale quando veniva visualizzato il messaggio &quot;Nessun grafico trovato&quot;
* Problema a causa del quale i valori di input per il parametro Offset rotazione nella feature Dimensioni fisiche non venivano modificati
* Problema a causa del quale le istanze del grafico duplicate avevano valori GraphID errati per gli input
* Problema a causa del quale il generatore di Substance non veniva inizializzato correttamente nell’editor durante l’utilizzo degli script dell’editor (finestra dell’editor personalizzato) per modificare un grafico
* Problema a causa del quale l’esportazione di un SubstanceGraphSO.CurrentStatePreset da uno script della finestra di un editor personalizzato ha esportato una versione memorizzata nella cache del grafico
* Problema a causa del quale le modifiche ai parametri non venivano salvate quando la finestra del controllo era bloccata
* Problema a causa del quale l’immissione manuale della tastiera nella sezione Scostamento posizione delle opzioni Dimensioni fisiche non aveva effetto sul materiale in modalità Editor
* Errore durante la digitazione manuale dei valori dei parametri nell&#39;oggetto SBSAR

## Unità 3.5.0

<b>Aggiunto/Aggiornato:</b>

* Supporto per consentire agli utenti di modificare il modo in cui le texture di output vengono assegnate al materiale Unity
* Compatibilità dei plug-in con la versione più recente di Unity 2022.2

<b>Corretto:</b>

* Errore di riferimento nullo quando i materiali hanno un input Int4
* Errore con input Int4. Il valore W viene assegnato a Data2 anziché a Data3.
* Errore nel nome della funzione &quot;\_OcclusionStrength&quot;

## Unità 3.4.0

<b>Aggiunto/Aggiornato:</b>

* Posizionate i controlli di scostamento per traslare la texture sulla superficie nel pannello dimensioni fisiche
* Collegamenti per scaricare Substance 3D Assets e Substance risorse della community nelle impostazioni del progetto

## Unità 3.3.0

<b>Aggiunto/Aggiornato:</b>

* La funzione dimensioni fisiche per HDRP, che consente di applicare e ridimensionare i materiali in base alle dimensioni reali
* Interfaccia utente per l&#39;abilitazione della GPU nelle impostazioni del progetto

<b>Rimosso:</b>

* graphID dalla maggior parte delle chiamate API

## Unità 3.2.1

<b>Corretto:</b>

* Problema relativo all’aggiornamento del plug-in dalla versione 3.0.0 e 3.1.0 alla versione più recente.

## Unità 3.2.0

<b>Aggiunto/Aggiornato:</b>

* Miglioramento delle prestazioni durante la ricompilazione degli script

<b>Corretto:</b>

* Importazione delle risorse non riuscita nel plug-in Unity durante l&#39;importazione di materiali Sbsar personalizzati
* Errore &quot;ArgumentException: il valore non rientra nell&#39;intervallo previsto&quot;
* Errore &quot;ArgumentOutOfRangeException: indice fuori intervallo&quot;

## Unità 3.1.0

<b>Aggiunto/Aggiornato:</b>

* Miglioramento delle prestazioni di 1,38x per Mac
* Il motore GPU su Mac utilizza Metal invece di OpenGL

<b>Corretto:</b>

* Problema di Mac in cui i canali R e B delle texture di output verranno capovolti

## Unità 3.0.0

<b>Aggiunto/Aggiornato:</b>

* Supporto per Apple Silicon
* Nuova esercitazione di YouTube su come utilizzare il plug-in
* Nuova documentazione sullo scripting

<b>Corretto:</b>

* Bug nella finestra di ispezione quando si preme ripetutamente il pulsante di selezione casuale
* Gli input di texture Null interrompono gli aggiornamenti delle Substance
* L’interruttore &quot;Genera tutti gli output&quot;, &quot;Genera mappe mappa mappa mappa&quot; e &quot;Solo runtime&quot; non funziona
* Problemi con gli spazi dei nomi
* Errore di riferimento nullo quando si entra in modalità di riproduzione con la risorsa del grafico selezionata
* Problema con HDRP e URP per la versione 2021.3 LTS più recente di Unity quando si utilizzano materiali solo di runtime
