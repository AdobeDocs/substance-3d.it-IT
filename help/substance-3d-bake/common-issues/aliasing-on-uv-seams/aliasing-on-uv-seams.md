---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: Correggi gli artefatti di alias visualizzati sulle giunture UV durante la cottura regolando le impostazioni di antialiasing e riempimento.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Alias sulle giunture UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Alias sulle giunture UV

>[!WARNING]
>
> **Problema**
> 
> Dopo la cottura al forno compaiono punti o macchie scure sul bordo delle giunture UV:
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **Spiegazione**
> 
> Quando il Baker scrive le informazioni nella texture, queste devono essere convertite da geometria a pixel. L&#39;elaborazione di queste informazioni potrebbe introdurre [aliasing](https://en.wikipedia.org/wiki/Aliasing). L&#39;alias si verifica spesso perché la geometria degli UV non è allineata alla griglia dei pixel o perché gli UV non coprono un numero di pixel sufficiente a fornire una risoluzione sufficiente.
> 
> Nelle immagini seguenti la geometria è la sovrapposizione rossa. Il fornaio contrassegna un pixel come pieno se più della metà della sua superficie è coperta dalla geometria (i quadrati bianchi sono pixel pieni e i quadrati neri sono pixel vuoti). Nell’immagine a destra, la griglia di pixel ha una risoluzione doppia e consente una rappresentazione più accurata della geometria.
> 
> ![](../../assets/aliasing-example-large.png)
> 
> ![](../../assets/aliasing-example-small.png)

>[!NOTE]
>
> **Soluzione**
> 
> * Aumentate la risoluzione della texture di output dei forni.
> * Aumentare l&#39;impostazione Anti-alias (nota: il calcolo potrebbe richiedere più tempo).
> * Allinea gli UV alla griglia pixel nell&#39;editor UV del software di modellazione 3D.
> * Offrite una migliore proporzione di texel rispetto agli UV.
