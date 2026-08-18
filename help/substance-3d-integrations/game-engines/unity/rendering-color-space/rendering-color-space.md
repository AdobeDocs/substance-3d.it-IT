---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/rendering-color-space.html"
breadcrumb-title: ''
description: Configura le impostazioni dello spazio colore di Unity per garantire il rendering corretto dei materiali Substance con ombreggiatori basati fisicamente.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Rendering Color Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Rendering dello spazio colore
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Rendering dello spazio colore

Le texture di Substance sono progettate per essere utilizzate con uno shader basato su dati fisici. Per risultati ottimali, imposta lo spazio colore su lineare in Impostazioni lettore unità.

1. Vai a Modifica>Impostazioni progetto>Lettore
1. Nella sezione Rendering, impostate lo Spazio colore su Lineare. (per impostazione predefinita, l’opzione Spazio gamma è errata e il colore della texture non sarà corretto).

   >[!NOTE]
   >
   > **Informazioni**
   > 
   > Le opzioni sRGB sulle texture sono disattivate se l’Impostazione dello spazio colore in Unità è impostata su Gamma

   ![](../../../assets/rendering-4.png){width="600px"}
