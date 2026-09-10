---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: Correggete gli artefatti di ombreggiatura del nero visibili sulle superfici della trama correggendo lo spazio tangente e i calcoli normali.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Sulla superficie della trama è visibile una croce di ombreggiatura nera
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# La croce di ombreggiatura nera è visibile sulla superficie della trama

Gli artefatti dell’ombreggiatura del nero appaiono su più aree della trama quando sono in condizioni di illuminazione.

![](../../assets/black-shading-cross.jpg)


## Descrizione

Una croce nera ombreggiata di solito significa che la mappa normale non corrisponde alla trama, in genere perché la geometria della trama è cambiata o è stata calcolata in modo diverso dal calcolo eseguito dal baker. Ad esempio: la triangolazione della trama è diversa tra il baker e la finestra della vista che esegue il rendering della trama e della relativa mappa normale.

## Soluzione

Assicurati che l’applicazione che mostra la trama e la relativa mappa normale siano sincronizzate con il modo in cui la texture è stata eseguita i baking. Ciò implica:

* Verificate che lo Spazio tangente sia identico tra il visualizzatore e il baker.
* Verificate che il formato Normale sia identico tra la vista e il baker.
* Verificate che la Triangolazione sia identica tra il visualizzatore e il baker. Per ulteriori informazioni, vedere [questa pagina](../../guides/triangulating-before-bak/triangulating-before-baking.md).
