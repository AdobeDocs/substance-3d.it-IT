---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: Risolvete la mappa colore dai fallimenti della cottura con trama controllando le proprietà del colore della trama e la mappatura UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Baking non riuscito con Mappa colori da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Baking non riuscito con Mappa colori da trama

>[!WARNING]
>
> **Problema**
> 
> Messaggio di errore possibile:
> 
> > > > 
> 
> [ Baking ] Baking non riuscito (Mappa colori da trama)\
> Impossibile trovare i colori dei vertici

>[!NOTE]
>
> **Spiegazione**
> 
> Le impostazioni predefinite per [Mappa colore da trama](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md) prevedono che i colori del vertice della trama ad alto poli vengano convertiti in una texture basata sugli UV della trama. Tuttavia, è spesso il caso in cui la trama ad alto poli non ha informazioni sui colori dei vertici. Pertanto il fornaio non può scrivere informazioni che non esistono.

>[!NOTE]
>
> **Soluzione**
> 
> Sono disponibili soluzioni diverse per evitare questo messaggio di errore:
> 
> * Usa una trama ad alto poli con i vertici colorati
> * Impostare la Mappa colore dal fornaio di trama con diverse impostazioni
> * Non usate la Mappa colore del fornaio di trama se non ne avete bisogno
