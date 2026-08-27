---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.html"
breadcrumb-title: ''
description: Scopri perché l’opzione Corrispondenza per nome non funziona con i forni di Occlusione ambiente e Thickness e trova alternative.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why is Matching by Name not working with Ambient OcclusionThickness "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Perché la funzione Corrispondenza per nome non funziona con OcclusioneSpessore ambiente '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 0%

---


# Perché la funzione Corrispondenza per nome non funziona con Occlusione/Thickness ambiente?

>[!WARNING]
>
> **Domanda**
> 
> Ho abilitato [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md) nei [parametri comuni](../../bakers-settings/common-parameters/common-parameters.md) per filtrare e ordinare le mie trame poly basse e alte, perché il fornaio di Occlusione ambiente lo ignora?

>[!NOTE]
>
> **Spiegazione**
> 
> I raggi secondari di avvio di Ambiente (Ambient Occlusioni), Thickness () e Normali piegati (Bent Normals) vengono visualizzati quando calcolano le texture. Questi raggi hanno la propria impostazione Corrispondenza per nome.

>[!NOTE]
>
> **Soluzione: Substance Painter**
> 
> Soluzione: abilitare il filtro corrispondenza per nome per i raggi secondari nei parametri baker.
