---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/modo/substance-in-modo-overview.html"
breadcrumb-title: ''
description: Scopri il plug-in Substance per MODO e come importare e utilizzare i materiali Substance nel tuo flusso di lavoro.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Substance in MODO Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panoramica di Substance in MODO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---


# Panoramica di Substance in MODO

## Panoramica:

## Apertura di una Substance

1. Create un materiale o selezionate un gruppo di materiali.
1. In Texture (Texture) > Substance (), scegliete Crea Substance o utilizzate il pulsante Crea (Create) nelle opzioni del kit di Substance. In questo modo viene creato un materiale di Substance nell&#39;albero dello shader.
1. Fare clic su Carica sbsar per caricare un file sbsar.

   ![](../../../assets/load-1.png)

## Creazione di output

Utilizzando la **modalità di Ombreggiatura predefinita basata su principi**, potete creare output utilizzando il flusso di lavoro metallizzato/rugosità.

1. Nella sezione Output delle proprietà della Substance, fai clic sugli output necessari per l’ombreggiatura. Verrà generata la texture della Substance, che verrà aggiunta all’albero shader con l’effetto livello materiale corretto. Per la modalità di Ombreggiatura basata su principi, è necessario disporre dei seguenti elementi:

   | Substance output | Spazio colore | Effetto Livello Di Materiale (Modalità Di Ombreggiatura Basata Su Principi) |
   | --- | --- | --- |
   | Colore di base | sRGB | Diffondi il colore |
   | Normale | Lineare | Normale |
   | Ruvidità | Lineare | Ruvidità |
   | Metallizzato | Lineare | Metallizzato |

   ![](../../../assets/outputs-3.png)

## Modifica della risoluzione e dei parametri

Potete modificare i parametri delle Substance per aggiornare o modificare le texture generate. Modificando un parametro, la Substance Engine ricalcolerà le texture che vengono introdotte nel materiale MODO.

1. Accedete a Proprietà Substance per il Materiale Substance e, nella sezione Modifiche, modificate uno qualsiasi dei parametri.

   ![](../../../assets/params.png)
1. Potete modificare la risoluzione delle texture generate utilizzando il menu a discesa Dimensione output. La Substance può essere impostata per generare fino a 8K. Per l&#39;output 8K è richiesto il motore [Substance GPU](../../../3d-applications/modo/modo-switch-engine/modo-switch-engine.md).
