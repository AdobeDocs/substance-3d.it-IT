---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/converting-substance-outputs.html"
breadcrumb-title: ''
description: Scopri come convertire gli output di materiale Substance in base ai diversi requisiti di rendering e flussi di lavoro.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Converting Substance outputs
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Conversione delle uscite Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# Conversione delle uscite Substance

## Substance Painter

Puoi esportare le mappe convertite da Substance Painter. È supportata una vasta gamma di predefiniti di rendering e la semplice selezione di un predefinito comporta la conversione dei tipi di mappe. (la conversione si basa sul flusso di lavoro metallo/grezzo).

![](../../assets/convertpainter.png){width="800px"}

## Substance plug-in

Il plug-in Substance genererà output e creerà automaticamente materiali per flussi di lavoro specifici. Tuttavia, con le applicazioni DCC e i moduli di rendering di terze parti, potrebbe essere necessario convertire manualmente gli output metallici o di prova. Le seguenti integrazioni supportano i flussi di lavoro di rendering automatico e, se necessario, convertiranno in modo appropriato qualsiasi tipo di mappa:

* [Substance a Maya](../../3d-applications/maya/using-workflows/using-workflows.md)
* [Substance in 3ds Max](../../3d-applications/3ds-max/3ds-max.md)

## Substance personalizzata

Se state creando una Substance personalizzata, potete creare gli output specifici necessari per i moduli di rendering come Vray e Corona. Utilizzando il nodo di conversione metallo/rugosità (Libreria>Utilità PBR), potete convertire facilmente il colore di base, la rugosità e le mappe metalliche nel modulo di rendering specifico.

![](../../assets/convert-designer.png){width="600px"}
