---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: Risolvete gli errori di esegue i baking delle Mappe colori da mesh controllando le proprietà dei colori della trama e la mappatura UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Esegue i baking non riuscita con Mappe colori da mesh
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Esegue i baking non riuscita con Mappe colori da mesh

>[!WARNING]
>
> **Problema**
> 
> Messaggio di errore possibile:
> 
> > > > 
> 
> [ Esegue i baking ] Esegue i baking non riuscita (Mappa colori da mesh)\
> Impossibile trovare i colori dei vertici

>[!NOTE]
>
> **Spiegazione**
> 
> Per impostazione predefinita, la [Mappa colori da mesh](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md) esegue i baking i colori dei vertici con trama ad alto poli in una texture basata sugli UV con trama. Tuttavia, è spesso il caso in cui la trama ad alto poli non ha informazioni sui colori dei vertici. Pertanto, il baker non può scrivere informazioni che non esistono.

>[!NOTE]
>
> **Soluzione**
> 
> Sono disponibili soluzioni diverse per evitare questo messaggio di errore:
> 
> * Usa una trama ad alto poli con i vertici colorati
> * Impostare il baker di Mappe colori da mesh con diverse impostazioni
> * Non usare il baker Mappa colori da mesh se non è necessario
