---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ''
description: Scopri il plug-in Substance per 3ds Max e come importare e utilizzare i materiali Substance nei tuoi progetti.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panoramica di Substance in 3ds Max
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Panoramica di Substance in 3ds Max

## Panoramica del plug-in:

## Apertura di una Substance

1. Aprire l&#39;editor Slate, cercare Substance e trascinare il nodo Substance2 nella visualizzazione.
1. Fare doppio clic sul nodo Substance per attivare le proprietà e in Substance Browser pacchetti caricare una Substance.

   >[!NOTE]
   >
   > È inoltre possibile trascinare il file con estensione sbsar nell&#39;editor di slate per creare automaticamente il nodo e importare la barra di slate.
1. Se una Substance contiene più grafici, potete scegliere il grafico da generare come materiale dal menu a discesa Grafico selezionato.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max8?$png$&jpegSize=100&wid=341)

   ![](../../../assets/max1.png)
1. Con il nodo Substance selezionato, accedi al menu Substance e scegli un modulo di rendering supportato. Il materiale verrà creato e pronto per essere applicato all&#39;oggetto. Le texture delle Substance sono collegate al materiale di rendering.

   | Rendering supportati |
   | --- |
   | Arnold |
   | Vray |
   | Corona |
   | Ottano |

   ![](../../../assets/max3.png)

## Modifica della risoluzione:

1. Impostate la risoluzione desiderata per le texture della Substance calcolata in Impostazioni output Substance.
1. Per una risoluzione fino a 8K, assicuratevi di utilizzare il motore GPU, impostato nelle [Impostazioni Substance](../../../3d-applications/3ds-max/settings-1/substance-settings.md).

   ![](../../../assets/max6.png)

## Modifica dei parametri:

1. Fate doppio clic sul nodo della Substance per caricare i parametri della Substance nella finestra dei parametri.
1. Modificate i parametri per aggiornare automaticamente le texture delle Substance.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## Impostazione dell&#39;anteprima di output:

È possibile impostare un canale specifico per la miniatura del nodo Substance.

1. Nel menu a discesa Anteprima output, scegli il canale che desideri utilizzare per la miniatura del nodo.

   ![](../../../assets/max7.png)

## Substance in porzioni:

Potete usare le proprietà Coordinate per suddividere le texture delle Substance e impostare i canali di mappatura.

![](../../../assets/max10.png)
