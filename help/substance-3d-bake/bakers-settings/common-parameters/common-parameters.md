---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: Scopri i parametri comuni che si applicano a tutti i baker e come configurarli per una generazione texture ottimale.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Common Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parametri comuni
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# Parametri comuni

I parametri comuni si applicano a tutti i baker. Questi parametri di solito definiscono il comportamento e il funzionamento dei baker con trame a poli elevato, ma anche la modalità di generazione delle texture finali. Alcuni di questi parametri possono essere sostituiti da baker specifici.

Sebbene la maggior parte di questi parametri sia disponibile in tutto il software (incluso Substance Automation Toolkit), il loro comportamento potrebbe essere leggermente diverso o alcuni potrebbero non essere disponibili a seconda del flusso di lavoro e dell&#39;implementazione del software.

## Parametri generali

Questi parametri influiscono sul modo in cui i baker generano le texture.

| *Nome* | *Descrizione* |
| --- | --- |
| **Dimensioni**(dimensioni predefinite o dimensioni di output) | Controlla la risoluzione della texture di output eseguita i baking (in pixel).Valori disponibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> (impostazione predefinita)</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>Sono supportate anche le risoluzioni non quadrate, ad esempio: 2048x1024 (rapporto 2:1). In Substance Designer questo parametro può essere sostituito dal baker stesso. |
| **Formato** | Formato file delle texture eseguite i baking.*Non disponibile nella versione di Substance Painter.* Vedere: [Come esportare le mappe con baking](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md). |
| **Antialiasing** | Controlla l’anti-alias che può migliorare la qualità della texture eseguita i baking e ridurre l’alias nei punti in cui si collegano geometrie diverse.Per ulteriori informazioni sull&#39;alias, vedere: [Alias sulle giunture UV](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) e [Alias su Wikipedia](https://en.wikipedia.org/wiki/Aliasing).Valori disponibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nessuno</strong> (impostazione predefinita)</li><li data-preserve-html="true"><strong>Sottocampionamento 2x2</strong></li><li data-preserve-html="true"><strong>Sottocampionamento 4x4</strong></li><li data-preserve-html="true"><strong>Sottocampionamento 8x8</strong></li></ul>  **Nota:** l&#39;attivazione dell&#39;antialiasing può aumentare notevolmente il tempo di cottura, poiché l&#39;antialiasing funziona calcolando la texture a una risoluzione più elevata e quindi ridimensionandola di nuovo alle dimensioni selezionate in origine. Ciò significa che una texture 2K con un subsampling 2x2 calcola effettivamente una texture 4K.A volte è preferibile aumentare il numero di raggi nel panettiere piuttosto che aumentare il subsampling. Si potrebbero ottenere risultati migliori senza attendere troppo. |
| **Set UV** | Controlla quali UV della trama a basso poli verranno utilizzati per calcolare le texture cotte.*Non disponibile nella versione di Substance Painter.* |
|  |  |
| **Dilatazione (px)** | Dilatate/estendete i pixel degli UV esterni o del loro bordo per la quantità di pixel specificata. Questa operazione consente di evitare giunture ai bordi UV quando questi bordi non sono perfettamente allineati ai pixel della texture o quando la risoluzione della texture viene ridotta (ad esempio: mipmaps). Si tratta di un processo di post-cottura applicato dopo il processo di cottura. A volte può essere chiamato anche &quot;padding&quot;.Per ulteriori informazioni sulla dilatazione, vedere: [Alias sulle giunture UV](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) e [Spaziatura interna](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/spdoc/padding-134643719.html). |
| **Applica diffusione** | Se questa opzione è attivata, l’esterno degli UV verrà riempito con colori sfumati in base ai bordi UV. Questo processo garantisce che quando la dimensione della texture viene ridotta, rimanga stabile e non crei giunture eccessivamente visibili (ad esempio, mipmap). Si tratta di un processo di post-cottura applicato dopo il processo di cottura. |
| **Normali medi** | Se attivata, calcola la normale media di un vertice per sapere in quale direzione inviare raggi durante il processo di mesh matching della cottura. Se è disattivata, i raggi seguiranno le normali dei vertici originali della trama. |

## Parametri High-Poly

I seguenti parametri controllano la cottura con rete ad alto e basso poli (&quot;da rete&quot;).

| *Nome* | *Descrizione* |
| --- | --- |
| **Trame ad alta definizione** | Un elenco di file (o risorse Substance pacchetto) che contiene trame a poligono elevato. Vengono caricati in memoria dai fornai quando il processo di cottura inizia a calcolare informazioni diverse e a salvare tali informazioni mesh nelle texture. Questo elenco viene ignorato se è abilitato &quot;**Usa definizione bassa**&quot;. |
| **Utilizzare Low come High Definition** o **Utilizzare Low Poly Mesh come High Poly Mesh** | Se questa opzione è attivata, l’elenco delle trame ad alto poli fornito ai panettieri viene ignorato e la trama a basso poli viene invece cotta su se stessa.Questo parametro è utile quando lavorate direttamente con una trama ad alto poli. Quando, ad esempio, si esegue la cottura in forno di una texture di occlusione ambientale per un&#39;auto di polo elevato con questa impostazione attivata, la distanza di raggio viene ignorata e il fornaio produrrà una cottura perfetta (nessun errore di raggio o mancata corrispondenza geometrica). |
|  |  |
| **Imposta distanza con gabbia** o **Usa gabbia** | Indica se utilizzare un file di mesh di gabbia nel processo di cottura al forno anziché i valori della distanza del raggio. La gabbia controlla la distanza e la direzione massima del raggio. |
| **File Cage** | Percorso del file mesh contenente la gabbia. |
| **Valore frontale** o **Distanza frontale massima** | Controlla quanto deve iniziare il raggio a trovare una geometria a poli alti lungo il tracciato al di sopra della superficie a poli bassi.*Questa impostazione non ha effetto quando si utilizza una gabbia.* |
| **Valore posteriore** o **Distanza posteriore massima** | Controlla la distanza al di sotto della superficie di poli bassi che il raggio deve arrestare per trovare qualsiasi geometria di poli alti lungo il suo tracciato.*Questa impostazione non ha effetto quando si utilizza una gabbia.* |
| **Rispetto al rettangolo di selezione** | Se attivato, la distanza di raggio e altri calcoli basati sulle dimensioni si basano sullo spazio normalizzato della trama a basso poli. Se è disattivata, il calcolo della distanza del raggio si basa sulle unità specificate nella trama a basso poli al momento dell&#39;esportazione (metri, centimetri, ecc.). A volte può essere utile disattivare questa impostazione e immettere manualmente la distanza del raggio quando un oggetto ha misure precise. |
|  |  |
| **Corrispondenza** | Indica in che modo i forni devono corrispondere alla geometria bassa e alta. Può essere utilizzato per filtrare il processo di cottura al forno senza la necessità di spostare manualmente (esplodere) le trame.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (impostazione predefinita): la trama a basso poli corrisponde a ogni trama a elevato poli.</li><li data-preserve-html="true"><strong>Per nome trama</strong>: filtrate le trame in base al nome per evitare che corrispondano a geometria indesiderata.</li></ul>Per ulteriori informazioni sulla geometria corrispondente, vedere: [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md). |
| **Suffissi corrispondenti** o **Suffisso trama poly alta** **Suffisso trama poly bassa** | Il nome della trama è suffisso per identificare e raggruppare la geometria quando si utilizza la feature Corrispondenza per nome (Matching By Name). Suffissi disponibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Low Poly Mesh</strong>: suffisso per identificare le trame poly basse nella scena</li><li data-preserve-html="true"><strong>Trama poly alta</strong>: suffisso per identificare le trame poly alte nella scena</li><li data-preserve-html="true"><strong>Ignora backfaces</strong>: suffisso per identificare trame che devono essere ignorate da specifici forni (ad esempio [Occlusione ambiente da trama](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md))</li></ul>Per ulteriori informazioni sulla geometria corrispondente, vedere: [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md) . |
|  |  |
| **Usa correzione inclinazione** | Se questa opzione è attivata, la direzione del raggio verrà calcolata a partire da **Normale medio** o dalla normale della geometria originale, a seconda della texture di input. I valori del nero nella texture utilizzano la normale media calcolata, mentre i valori del bianco utilizzano la normale della trama originale.*Non disponibile nella versione di Substance Painter.* |
| **Inclina mappa** | Percorso del file di texture utilizzato per inclinare la proiezione dei raggi. |
| **Inverti correzione inclinazione** | Invertite la lettura della texture di input (il nero diventa bianco e il bianco diventa nero). |
