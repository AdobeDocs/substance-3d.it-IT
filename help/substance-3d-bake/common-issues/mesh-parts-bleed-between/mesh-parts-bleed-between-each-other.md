---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: Impedire che le parti della trama si riversino reciprocamente durante la esegue i baking utilizzando Corrispondenza per nome o regolando le distanze.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Le parti della trama sanguinano tra loro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# Le parti della trama sanguinano tra loro

>[!WARNING]
>
> **Problema**
> 
> La geometria della trama sanguina su altre parti e crea artefatti.
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **Spiegazione**
> 
> Il processo di eseguita i baking invia raggi dalla superficie della trama a basso poli per colpire la trama a alto poli e creare una corrispondenza. A volte i raggi vanno troppo lontano e colpiscono la geometria sbagliata, creando il sanguinamento e gli artefatti.

>[!NOTE]
>
> **Soluzione**
> 
> Sono disponibili alcune soluzioni per evitare questo problema:
> 
> * Utilizza la funzione [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md) per isolare le trame
> * Utilizzate una [gabbia](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) per limitare la distanza dei raggi.
> * Impostate a un valore inferiore la distanza di raggio predefinita nelle impostazioni di baker comuni.
