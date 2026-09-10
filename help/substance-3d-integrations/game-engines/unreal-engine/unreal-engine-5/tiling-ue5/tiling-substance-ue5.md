---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/tiling-substance-ue5.html"
breadcrumb-title: ''
description: Affianca texture Substance in Unreal Engine 5 aggiungendo nodi di coordinate Texture e parametri scalari ai materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Tiling Substance - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance Affiancamento - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# Substance Affiancamento - UE5

Per affiancare una texture Substance, dovrete aggiungere un nodo Coordinate Texture e moltiplicarlo per il parametro scalare.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

Per creare parametri sia per il riquadro U che per il riquadro V, è possibile utilizzare un vettore Append e moltiplicarlo per il TexCoord. Ciò consente di impostare in modo indipendente le quantità delle porzioni U e V.

![](../../../../assets/tiling-3.png){width="800px"}
