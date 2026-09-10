---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: Scoprite le differenze tra OpenGL e i formati mappa normali e quando usarli ciascuno.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Qual è la differenza tra OpenGL e il formato normale DirectX? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# Qual è la differenza tra OpenGL e il formato normale DirectX?

>[!WARNING]
>
> **Domanda**
> 
> Qual è la differenza tra OpenGL e il formato normale DirectX?

>[!NOTE]
>
> **Spiegazione**
> 
> OpenGL e DirectX sono due API grafiche (set di funzioni) che i programmatori utilizzano nella loro applicazione per dialogare con la GPU (Graphic Processing Unit). In termini di mappe normali, la differenza determina come deve essere interpretato il canale verde di una texture RGB. OpenGL prevede che il primo pixel si trovi nella parte inferiore, mentre DirectX prevede che si trovi nella parte superiore. Questo è spesso il motivo per cui in varie discussioni tecniche si consiglia di provare a invertire il canale verde di una mappa normale per vedere se si comporta meglio mentre inverte i valori dei pixel (prima diventa ultima). OpenGL può essere indicato come **Y+** (bottom-up) mentre DirectX come **Y-** (top-down).
> 
> Per sapere quale formato utilizzare, fate riferimento all’applicazione di destinazione in cui verranno utilizzate le texture.
