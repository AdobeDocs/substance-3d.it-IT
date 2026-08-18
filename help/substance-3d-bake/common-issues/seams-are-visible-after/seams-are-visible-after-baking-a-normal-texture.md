---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: Eliminate le giunture visibili nelle texture normali cotte regolando l'imbottitura, l'anti-alias e il layout UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Le cuciture sono visibili dopo la cottura di una texture normale
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Le cuciture sono visibili dopo la cottura di una texture normale

>[!WARNING]
>
> **Problema**
> 
> Le normali giunture delle mappe sono visibili ai bordi UV della trama anche dopo un forno pulito.

>[!NOTE]
>
> **Spiegazione**
> 
> Anche dopo una cottura perfetta, le cuciture possono ancora essere visibili. Il motivo principale è che una normale approssimazione delle informazioni di superficie in una texture. A volte la texture manca di precisione o deve compensare troppo tra la geometria poly bassa e quella alta per essere abbastanza accurata. In altre situazioni, il modo in cui la geometria viene orientata con la sua mappa normale può influire sul suo aspetto ottimale.

>[!NOTE]
>
> **Soluzione**
> 
> Si possono provare alcune soluzioni possibili per ridurre l&#39;intensità delle cuciture con mappe normali:
> 
> * Spesso gli UV non sono allineati ai pixel, il che porta all&#39;aliasing e produce giunture. Per ulteriori informazioni, vedere [questa pagina](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md).
>   * Aumentando la risoluzione della texture si può ridurre questo effetto.
>   * Allineando i bordi UV ai pixel è possibile ridurre questo effetto.
> * Aumentate l&#39;impostazione dello shader **qualità**. La qualità dello shader può influire sul modo in cui vengono calcolati i riflessi di specular. Se alcune Isole UV vengono ruotate e questo parametro è troppo basso, possono verificarsi giunture visibili. Per ulteriori informazioni, vedere [questa pagina](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html).
