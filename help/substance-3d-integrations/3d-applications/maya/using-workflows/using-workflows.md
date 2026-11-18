---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ""
description: Creazione e utilizzo di predefiniti di rendering per gli output Substance in Maya per generare automaticamente reti di shader per diversi moduli di rendering.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo dei flussi di lavoro
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%
---

# Utilizzo dei flussi di lavoro

In Flussi di lavoro, puoi scegliere o creare predefiniti di rendering per gli output di Substance. Questi predefiniti sono reti di shader per un modulo di rendering come Arnold o Vray.

>[!NOTE]
>
> **Posizioni predefinite flusso di lavoro**
>
> **Windows**:
> C:\Users\\Documents\maya\2022\substance\workflows\generated
> **MacOS**:
> /Utenti//Libreria/Preferenze/Autodesk/maya//substance/workflow/generated
> **Linux**:
> /home//maya//substance/workflows/generated

![](../../../assets/maya-max-v3-1/maya-all-presets.png)

Per utilizzare un flusso di lavoro, è sufficiente scegliere il predefinito dall’elenco e quindi fare clic sul pulsante Crea rete.

![](../../../assets/workflow.gif)

## Creazione di un flusso di lavoro

Potete creare un flusso di lavoro personalizzato e aggiungerlo all’elenco Flusso di lavoro modulo di rendering. Quando si aggiunge un nuovo flusso di lavoro, tutti i nodi creati dopo il nodo Substance verranno salvati nel flusso di lavoro. Ciò consente di creare un numero qualsiasi di nodi di ombreggiatura per creare una rete di shader personalizzata completa che può essere salvata come flusso di lavoro predefinito.

![](../../../assets/saved-workflow.png)

## Gestione dei workflow

### Salvataggio dei flussi di lavoro personalizzati

1. Create manualmente gli output delle Substance e collegateli a un materiale come aiStandardSurface.
   1. Per creare la rete di shader, potete utilizzare qualsiasi nodo Maya o eseguire il rendering di nodi specifici.
1. Fai clic sul pulsante **Crea flusso di lavoro** e immetti un nome per il predefinito del flusso di lavoro.

### Duplicazione dei flussi di lavoro

È possibile duplicare un flusso di lavoro facendo clic sul pulsante **Duplica flusso di lavoro**.

### Rinomina e sovrascrivi flussi di lavoro

È possibile rinominare i flussi di lavoro esistenti e sovrascrivere i flussi di lavoro con i dati aggiornati utilizzando i pulsanti **Rinomina** e **Sovrascrivi** selezionati.

### Rimozione dei flussi di lavoro

È possibile rimuovere i flussi di lavoro esistenti utilizzando il pulsante Rimuovi flusso di lavoro.

## Flussi di lavoro di OpenPBR

Nell&#39;elenco Flussi di lavoro sono disponibili due flussi di lavoro OpenPBR: **OpenPBR** e **OpenPBR - V-Ray**. Questi flussi di lavoro sono progettati per l’uso con file SBSAR creati utilizzando l’modello di materiale in Substance 3D Designer o Sampler (OpenPBR è stato il modello predefinito dai tempi di Designer V16.0+ e Sampler V6.0+).

### Che cos’è l’OpenPBR

OpenPBR è un modello di ombreggiatura di materiali aperto e basato su elementi fisici sviluppato da Adobe e Autodesk e contribuito ad Academy Software Foundation (ASWF). Fornisce una definizione di materiale unificata compatibile tra i moduli di rendering. Per ulteriori informazioni, consulta la [documentazione OpenPBR](https://experienceleague.adobe.com/it/docs/substance-3d/general-knowledge/openpbr/openpbr-overview).

### Quando utilizzare un flusso di lavoro OpenPBR

Utilizza un flusso di lavoro di OpenPBR quando il file SBSAR è stato creato utilizzando l’OpenPBR in Substance 3D Designer o Substance 3D Sampler. Se SBSAR è stato creato utilizzando Adobe Standard modello di materiale (ASM), utilizzate il flusso di lavoro legacy compatibile con il modulo di rendering (Arnold, V-Ray o V-Ray 6).

>[!NOTE]
>
> Se si applica un flusso di lavoro di OpenPBR a un materiale ASM o un flusso di lavoro standard a un OpenPBR SBSAR, il plug-in collega solo gli output comuni a entrambi i modelli di materiale. Il risultato può essere incompleto.

### Flussi di lavoro di OpenPBR disponibili

**OpenPBR**

Utilizza il nodo Maya openPBRSurface nativo. Compatibile con Arnold e V-Ray. Questo è il flusso di lavoro consigliato per la maggior parte degli utenti che utilizzano materiali OpenPBR in Maya.

**OpenPBR - V-Ray**

Utilizza il materiale a raggi V (VRayMtl) in modalità di OpenPBR. Opzione consigliata per gli utenti la cui pipeline è specificamente creata in base alle impostazioni del materiale V-Ray.

### Come applicare un flusso di lavoro OpenPBR

1. Carica il file SBSAR nel plug-in usando il pulsante Carica Substance.
1. Nell&#39;elenco Flussi di lavoro, selezionare **OpenPBR** o **OpenPBR - V-Ray**.
1. Fare clic su **Crea rete** per creare la rete di shader nell&#39;**Editor materiale Hypershade**.
1. Il plug-in collega automaticamente le uscite SBSAR agli ingressi corrispondenti del nodo di OpenPBR.
1. Assegna il materiale alla trama come di consueto.

![](../../../assets/maya-max-v3-1/maya-openpbr-overview.png)
