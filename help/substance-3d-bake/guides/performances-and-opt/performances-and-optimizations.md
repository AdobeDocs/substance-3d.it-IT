---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/guides/performances-and-optimizations.html"
breadcrumb-title: ''
description: Scopri come ottimizzare la configurazione hardware e la preparazione della trama per ottenere prestazioni di esegue i baking più rapide.
helpx_creative_field: ""
helpx_description: bakers > Guides > Performances and optimizations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Prestazioni e ottimizzazione
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---


# Prestazioni e ottimizzazione

## Requisiti hardware minimi

Non esistono requisiti minimi per l&#39;uso di Substance Bakers, tuttavia è importante tenere presente quanto segue:

* Una buona CPU offre tempi di calcolo ridotti (più core velocizzano il calcolo di **dalla trama** baker che utilizzano il raytracing).
* Una discreta quantità di memoria (RAM) consentirà di caricare trame con molti dettagli (poligoni).
* Una buona GPU consentirà di generare texture a grandi risoluzioni (come 8K).

## Triangolazione

I baker funzionano internamente con trame triangolate; se i modelli 3D (poly basso e alto) non sono triangolati, i baker triangoleranno le trame stesse. Questo processo può richiedere molto tempo e aumenterà in modo lineare in relazione alla quantità di poligoni contenuti nel modello. Si consiglia in genere di triangolare le maglie (specialmente la trama poly alta) per evitare che questo processo si verifichi durante la eseguita i baking.

Se il flusso di lavoro è basato su FBX, potete triangolare la trama al momento dell’esportazione utilizzando un’opzione nell’applicazione DCC.

## Cache geometria

Per ulteriori informazioni, vedere la pagina seguente: [Cache geometria](../../features/geometry-cache/geometry-cache.md)

## Anti-alias

I baker possono utilizzare il super sampling per eseguire l’anti-alias. Con il supersampling, i baker emettono più raggi per pixel per arrotondare il risultato. Questa impostazione può influire notevolmente sul tempo di eseguita i baking; questo vale in particolare per i baker in cui sono necessari molti raggi, come l’occlusione ambientale dal baker mesh.

Ad esempio:

* Un&#39;impostazione AA di 2x2 indica che il baker emetterà una quantità di raggi 4 volte superiore a quella iniziale. Per una texture da 2048\*2048 px, il calcolo risultante equivale a eseguire i baking una texture da 4096\*4096 px e dovrebbe richiedere circa 4 volte più tempo per il calcolo.
* Un&#39;impostazione AA di 8x8 indica che il baker emette 64 volte la quantità iniziale di raggi. Per una texture da 2048\*2048 px, il tempo di calcolo risultante equivale a eseguire i baking una texture da 16384\*16384px e dovrebbe impiegare circa 64 volte più tempo per il calcolo.

**Tenendo conto di questi numeri, è necessario utilizzare con attenzione l&#39;impostazione 8x8**.

Per ridurre la presenza di rumore, si consiglia in genere di aumentare il numero di raggi secondari (per i baker di occlusione ambientale, thickness e normali incurvate) e di mantenere un&#39;impostazione AA 2x2 o 4x4 invece di utilizzare una quantità ridotta di raggi secondari e un&#39;impostazione AA elevata.

>[!NOTE]
>
> Una buona impostazione di prestazioni/qualità per l&#39;occlusione ambientale dalla trama consiste nell&#39;utilizzare AA 2x2 e almeno 128 raggi secondari.

## Formato file

L’esportazione dei file su disco può richiedere molto tempo a seconda del formato del file, della risoluzione, della profondità di bit e delle impostazioni di compressione. Le impostazioni di compressione possono essere modificate nelle opzioni Preferenze / Progetti / Generali / Formato file. Se si disattiva la compressione, i tempi di esportazione possono diminuire quando si espandono file di grandi dimensioni.

## ARRESTI ANOMALI e TDR

Gli Arresti anomali possono essere causati da più fattori, uno dei quali è il TDR (Timeout Detection Recovery). Il TDR è un meccanismo di Windows creato per rilevare e ripristinare le situazioni in cui la GPU sembra non rispondere. A causa di un basso valore predefinito per il rilevamento del ritardo TDR, è possibile riscontrare arresti anomali quando si utilizzano baker specifici in alcune situazioni:

* quando si eseguono i baking trame dense con il baker di Occlusione ambientale
* quando si utilizzano baker con accelerazione DXR a maglie di poli molto dense e alte (più di 60 milioni di triangoli)

Puoi trovare ulteriori informazioni sul TDR e una guida dettagliata su come modificare le impostazioni associate qui: [arresto anomalo di driver GPU con calcoli lunghi (arresto anomalo TDR)](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)
