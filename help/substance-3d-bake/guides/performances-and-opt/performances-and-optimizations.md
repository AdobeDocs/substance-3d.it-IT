---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/performances-and-optimizations.html"
breadcrumb-title: ''
description: Scoprite come ottimizzare la configurazione hardware e la preparazione della trama per ottenere prestazioni di cottura più rapide.
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

* Una buona CPU offre tempi di calcolo ridotti (più core velocizzano il calcolo di **dalla trama** dei forni che utilizzano il ray tracing).
* Una discreta quantità di memoria (RAM) consentirà di caricare trame con molti dettagli (poligoni).
* Una buona GPU consentirà di generare texture a grandi risoluzioni (come 8K).

## Triangolazione

I panettieri lavorano internamente con trame triangolate; se i modelli 3D (low e high poly) non sono triangolati, i panettieri triangoleranno essi stessi le trame. Questo processo può richiedere molto tempo e aumenterà in modo lineare in relazione alla quantità di poligoni contenuti nel modello. Si consiglia in genere di triangolare le maglie (specialmente la maglia poly alta) per evitare che questo processo si verifichi durante la cottura al forno.

Se il flusso di lavoro è basato su FBX, potete triangolare la trama al momento dell’esportazione utilizzando un’opzione nell’applicazione DCC.

## Cache geometria

Per ulteriori informazioni, vedere la pagina seguente: [Cache geometria](../../features/geometry-cache/geometry-cache.md)

## Anti-alias

I fornai possono utilizzare il super sampling per eseguire l’anti-alias. Il supersampling significa che i fornai emetteranno più raggi per pixel per uniformare il risultato. Il tempo di cottura può essere notevolmente influenzato da questa impostazione; questo è particolarmente vero per i forni in cui sono richiesti molti raggi, come l&#39;occlusione ambientale dal fornaio a rete.

Ad esempio:

* Un&#39;impostazione AA di 2x2 significa che il fornaio emette una quantità di raggi 4 volte superiore a quella iniziale. Per una texture di 2048\*2048 px, il calcolo risultante equivale alla cottura in forno di una texture di 4096\*4096px e dovrebbe richiedere circa 4 volte più tempo per il calcolo.
* Un&#39;impostazione AA di 8x8 significa che il fornaio emette una quantità di raggi 64 volte superiore a quella iniziale. Per una texture di 2048\*2048 px, il tempo di calcolo risultante è equivalente alla cottura in forno di una texture di 16384\*16384px e dovrebbe richiedere circa 64 volte più tempo per il calcolo.

**Tenendo conto di questi numeri, è necessario utilizzare con attenzione l&#39;impostazione 8x8**.

Per ridurre la presenza di rumore, si consiglia in genere di aumentare il numero di raggi secondari (per l&#39;occlusione ambientale, i forni standard per il thickness e la curvatura) e di mantenere un&#39;impostazione AA 2x2 o 4x4 piuttosto che utilizzare una quantità bassa di raggi secondari e un&#39;impostazione AA elevata.

>[!NOTE]
>
> Una buona impostazione di prestazioni/qualità per l&#39;occlusione ambientale dalla trama consiste nell&#39;utilizzare AA 2x2 e almeno 128 raggi secondari.

## Formato file

L’esportazione dei file su disco può richiedere molto tempo a seconda del formato del file, della risoluzione, della profondità di bit e delle impostazioni di compressione. Le impostazioni di compressione possono essere modificate nelle opzioni Preferenze / Progetti / Generali / Formato file. Se si disattiva la compressione, i tempi di esportazione possono diminuire quando si espandono file di grandi dimensioni.

## Arresti anomali e TDR

Gli arresti anomali possono essere causati da diversi fattori, tra cui il TDR (Timeout Detection Recovery). Il TDR è un meccanismo di Windows creato per rilevare e ripristinare le situazioni in cui la GPU sembra non rispondere. A causa di un basso valore predefinito per il rilevamento del ritardo TDR, si possono verificare arresti anomali quando si utilizzano specifici forni in alcune situazioni:

* quando si cuociono trame dense con il fornaio a Occlusione ambiente
* quando si utilizzano forni accelerati DXR con maglie poly molto dense (più di 60 milioni di triangoli)

Puoi trovare ulteriori informazioni sul TDR e una guida dettagliata su come modificare le impostazioni associate qui: [Arresto anomalo dei driver GPU con calcoli lunghi (arresto anomalo del TDR)](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)
