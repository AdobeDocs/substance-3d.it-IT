---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/using-workflows-in-3ds-max.html"
breadcrumb-title: ""
description: Utilizza i flussi di lavoro di rendering in 3ds Max per creare automaticamente reti di shader per diversi moduli di rendering dai materiali Substance.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Using Workflows in 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo dei flussi di lavoro in 3ds Max
user-guide-description: ""
user-guide-title: ""
source-git-commit: 335f3107fb325bb769325bff8c150b3e8b7ff054
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%
---

# Utilizzo dei flussi di lavoro in 3ds Max

Il plug-in Substance in 3ds Max contiene flussi di lavoro per la creazione automatica di una rete di shader per supportare i moduli di rendering. I flussi di lavoro di rendering si trovano nel menu Substance.

![](../../../assets/maya-max-v3-1/3dsmax-all-presets.png)

Per utilizzare un flusso di lavoro, selezionate il nodo Substance nell&#39;editor materiale e scegliete il flusso di lavoro dal menu Substance.

![](../../../assets/max-workflow.gif)

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
