---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-bump-offset-parallax-ue4.html"
breadcrumb-title: ''
description: Utilizzate la mappatura Scostamento rilievo con i materiali Substance in Unreal Engine 4 per creare l'illusione della profondità e i dettagli della superficie.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Bump Offset (Parallax) - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo dello scostamento rilievo (parallasse) - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Utilizzo dello scostamento rilievo (parallasse) - UE4

La mappatura **Scostamento rilievo** dà a una superficie l&#39;illusione della profondità modificando le coordinate UV in modo creativo per aiutare a spostare ulteriormente i testicoli dalla superficie dell&#39;oggetto, dando l&#39;illusione che la superficie abbia più dettagli di quanto non abbia in realtà. In questo esempio di procedura, non solo illustreremo come trovare l’espressione di materiale Scostamento rilievo, ma anche come utilizzare il nodo Scostamento rilievo nei Materiali.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/HowTo/BumpOffset/>

Per utilizzare l&#39;output di height, è necessario fare doppio clic sull&#39;output nell&#39;istanza di Substance Factory per creare il height. Height non è attivato per impostazione predefinita. Puoi quindi trascinare questo output di height nel materiale.

![](../../../../assets/height-1.png){width="600px"}

Create un nodo di scostamento rilievo, quindi collegate il canale Rosso del height al Height. È quindi possibile inserire un valore TexCoord nell&#39;input Coordinate dell&#39;offset di rilievo. Infine, l’output dello scostamento rilievo viene inserito nell’input UV per tutte le texture della Substance.

![](../../../../assets/bump.png){width="800px"}
