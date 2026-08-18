---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/corona.html"
breadcrumb-title: ''
description: Utilizza i materiali Substance con il modulo di rendering Corona in 3ds Max utilizzando il flusso di lavoro Specular/lucidità e le mappe richieste.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corona
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---


# Corona

Per il rendering con Corona puoi utilizzare le mappe esportate da Substance Painter o dal plug-in Substance. Corona utilizza il flusso di lavoro Specular/lucidità con una mappa 1/IOR. Avrai bisogno delle seguenti mappe:

* Diffusione
* Riflesso (Specular)
* Lucidità
* 1/IOR (convertito)

La mappa 1/IOR può essere convertita solo dal flusso di lavoro metallizzato/rugosità che è il flusso di lavoro predefinito sia nel Substance Designer che nella Substance Painter.

1. Esporta le mappe da Substance Painter utilizzando il predefinito Corona.
1. Per la Substance personalizzata, potete utilizzare il nodo convertito colore di base\_metallizzato\_rugosità impostato sul predefinito Vray per creare gli output personalizzati.
1. Per 3ds Max e Cinema 4D, utilizzi un materiale Corona a strati per gestire materiali metallici e dielettrici e bypassare la necessità di convertire una mappa 1/IOR.

## Sommario

* [Corona per 3ds Max](../../renderers/corona/corona-for-3ds-max/corona-for-3ds-max.md)
* [Corona - Substance Painter](../../renderers/corona/corona-painter/corona-substance-painter.md)
