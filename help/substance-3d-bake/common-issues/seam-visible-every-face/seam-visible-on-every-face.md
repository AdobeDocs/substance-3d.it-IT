---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: Correggi le giunture visibili su ogni volto verificando lo srotolamento UV, i gruppi di arrotondamento e i problemi relativi alla topologia della trama.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Cucitura visibile su ogni volto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Cucitura visibile su ogni volto

>[!WARNING]
>
> **Problema**
> 
> Una giuntura è visibile su alcuni bordi della geometria anche se non sono presenti giunture UV:
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **Spiegazione**
> 
> Se non si utilizza una [gabbia](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html), il processo di cottura avvia i raggi nella direzione delle normali dei vertici della trama a basso poli. Se le normali di ciascun vertice sono divise (ossia ogni faccia non condivide le stesse normali dei vertici della faccia vicina), i raggi non saranno inviati nella stessa direzione sugli spigoli. Ciò comporta la divisione, in quanto le informazioni su ciascun lato degli spigoli sono diverse.
> 
> Questo problema è aggravato anche dall&#39;alias, come spiegato in [questa pagina](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md).

>[!NOTE]
>
> **Soluzione**
> 
> In questo caso sono possibili solo due soluzioni:
> 
> * Utilizzate una [gabbia](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) per controllare la direzione del raggio invece di consentire al fornaio di calcolarla dalla geometria a basso poli.
> * Unite le normali dei vertici della trama a basso poli (ammorbiditele/applicate un gruppo di arrotondamento comune).
