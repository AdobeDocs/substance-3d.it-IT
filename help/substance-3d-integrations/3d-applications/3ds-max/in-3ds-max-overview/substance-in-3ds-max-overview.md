---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
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
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '653'
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

## Flussi di lavoro di OpenPBR

Nell&#39;elenco **Flussi di lavoro** del **menu Substance** sono disponibili due flussi di lavoro di OpenPBR: **Substance in OpenPBR** e **Substance in OpenPBR a raggi V**. Questi flussi di lavoro sono progettati per l’uso con file SBSAR creati utilizzando l’modello di materiale in Substance 3D Designer o Sampler (OpenPBR è stato il modello predefinito dai tempi di Designer V16.0+ e Sampler V6.0+).

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-node-preview.png)

### Che cos&#39;è l&#39;OpenPBR?

OpenPBR è un modello di ombreggiatura di materiali aperto e basato su elementi fisici sviluppato da Adobe e Autodesk e contribuito ad Academy Software Foundation (ASWF). Fornisce una definizione di materiale unificata compatibile tra i moduli di rendering. Per ulteriori informazioni, consulta la [documentazione OpenPBR](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/openpbr/openpbr-overview).

### Quando utilizzare un flusso di lavoro OpenPBR

Utilizza un flusso di lavoro di OpenPBR quando il file SBSAR è stato creato utilizzando l’OpenPBR in Substance 3D Designer o Substance 3D Sampler. Se SBSAR è stato creato utilizzando Adobe Standard modello di materiale (ASM), utilizzate il flusso di lavoro legacy compatibile con il modulo di rendering (Arnold, V-Ray o V-Ray 6).

>[!NOTE]
>
> Se si applica un flusso di lavoro di OpenPBR a un materiale ASM o un flusso di lavoro standard a un OpenPBR SBSAR, il plug-in collega solo gli output comuni a entrambi i modelli di materiale. Il risultato può essere incompleto.

### Flussi di lavoro di OpenPBR disponibili

**OpenPBR**

Utilizza il nodo 3ds Max openPBRSurface nativo. Compatibile con Arnold e V-Ray. Questo è il flusso di lavoro consigliato per la maggior parte degli utenti che utilizzano materiali OpenPBR in 3ds Max.

**OpenPBR - V-Ray**

Utilizza il materiale a raggi V (VRayMtl) in modalità di OpenPBR. Opzione consigliata per gli utenti la cui pipeline è specificamente creata in base alle impostazioni del materiale V-Ray.

### Come applicare un flusso di lavoro OpenPBR

![](../../../assets/maya-max-v3-1/3dsmax-substance-to-openpbr.png)

1. Seleziona il file SBSAR (OpenPBR) usando il pulsante Carica Substance.
1. Nel menu superiore, seleziona OpenPBR o OpenPBR - V-Ray.
1. Fare clic su Crea rete per creare la rete di shader nell&#39;Editor materiale di slate.
1. Il plug-in collega automaticamente le uscite SBSAR agli ingressi corrispondenti del nodo di OpenPBR.
1. Assegna il materiale alla trama come di consueto.

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-overview.png)
