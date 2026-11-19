---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ""
description: Scopri il plug-in Substance per 3ds Max e come importare e utilizzare i materiali Substance nei tuoi progetti.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panoramica di Substance in 3ds Max
user-guide-description: ""
user-guide-title: ""
source-git-commit: a167bcd2c2f0af70b3a4dc37eafc85145c79c590
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%
---

# Panoramica di Substance in 3ds Max

## Panoramica del plug-in

## Apertura di una Substance

1. Aprire l&#39;editor Slate, cercare Substance e trascinare il nodo Substance2 nella visualizzazione.
1. Fare doppio clic sul nodo Substance per attivare le proprietà e in Substance Browser pacchetti caricare una Substance.

   >[!NOTE]
   >
   > È inoltre possibile trascinare il file con estensione sbsar nell&#39;editor di slate per creare automaticamente il nodo e importare la barra di slate.

1. Se una Substance contiene più grafici, potete scegliere il grafico da generare come materiale dal menu a discesa Grafico selezionato.

   ![](../../../assets/max1.png)

1. Con il nodo Substance selezionato, accedi al menu Substance e scegli un modulo di rendering supportato. Il materiale verrà creato e pronto per essere applicato all&#39;oggetto. Le texture di Substance sono collegate al materiale di rendering.

>[!NOTE]
>
> Una volta selezionato il nodo **&quot;Substance 2&quot;**, è necessario fare clic prima sul nodo **Carica Substance...** per selezionare un file sbsar, quindi selezionare un modulo di rendering supportato dal menu superiore (ad esempio &quot;Substance ad Arnold&quot;).
>
>I moduli di rendering supportati includono Arnold, V-Ray, Corona e Octane. [Scopri i flussi di lavoro in 3DS Max per scoprire come utilizzare i materiali OpenPBR.](../using-workflows-3ds-max/using-workflows-in-3ds-max.md)

![](../../../assets/max3.png)

## Modifica della risoluzione

1. Impostate la risoluzione desiderata per le texture Substance calcolate in Impostazioni output Substance.
1. Per una risoluzione fino a 8K, assicuratevi di utilizzare il motore GPU, impostato nelle [Impostazioni Substance](../../../3d-applications/3ds-max/settings-1/substance-settings.md).

   ![](../../../assets/max6.png)

## Modifica dei parametri

1. Fate doppio clic sul nodo della Substance per caricare i parametri della Substance nella finestra dei parametri.
1. Modificate i parametri per aggiornare automaticamente le texture delle Substance.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## Impostazione dell’anteprima di output

È possibile impostare un canale specifico per la miniatura del nodo Substance.

1. Nel menu a discesa Anteprima output, scegli il canale che desideri utilizzare per la miniatura del nodo.

   ![](../../../assets/max7.png)

## Substance Affiancamento

È possibile utilizzare le proprietà Coordinate per affiancare texture di Substance e impostare Mapping canali.

![](../../../assets/max10.png)
