---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/tiling-substance-ue4.html"
breadcrumb-title: ''
description: Affianca le texture Substance in Unreal Engine 4 aggiungendo i nodi delle coordinate della texture e i parametri scalari ai materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Tiling Substance - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance in porzioni - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '77'
ht-degree: 0%

---


# Substance in porzioni - UE4

Per affiancare una texture di una sostanza, dovete aggiungere un nodo di coordinate della texture e moltiplicarlo per un parametro scalare.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

Per creare parametri sia per il riquadro U che per il riquadro V, è possibile utilizzare un vettore Append e moltiplicarlo per il TexCoord. Ciò consente di impostare in modo indipendente le quantità delle porzioni U e V.

![](../../../../assets/tiling-3.png){width="800px"}
