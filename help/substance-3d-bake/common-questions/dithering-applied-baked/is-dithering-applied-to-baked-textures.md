---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: Capite se il dithering viene applicato alle texture cotte e come incide sulla qualità della texture.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Il dithering viene applicato alle texture cotte '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Il dithering viene applicato alle texture cotte?

>[!WARNING]
>
> **Domanda**
> 
> I forni supportano il dithering [della texture](https://en.wikipedia.org/wiki/Dither) e, in caso affermativo, quando viene applicato?

>[!NOTE]
>
> **Spiegazione**
> 
> Il dithering viene applicato per evitare bande nelle mappe normali a 8 bit, ad esempio:
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **Soluzione: Substance Designer**
> 
> Il dithering viene applicato automaticamente nelle seguenti situazioni:
> 
> * Quando un output Baker viene salvato in un file texture a 8 bit
> * Quando un output Baker viene utilizzato in un nodo bitmap di un grafico impostato su 8 bit.

>[!NOTE]
>
> **Soluzione: Substance Painter**
> 
> Il dithering è un’opzione che può essere attivata o disattivata durante il processo di esportazione. Viene applicato solo quando si esporta in formato file a 8 bit per il canale Normale, Spostamento e Height.

>[!NOTE]
>
> **Soluzione: Substance Automation Toolkit**
> 
> Al momento il dithering non è supportato.
