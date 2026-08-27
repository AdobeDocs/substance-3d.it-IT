---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ''
description: Crea e utilizza i predefiniti di rendering per gli output Substance in Maya per generare automaticamente reti di shader per diversi moduli di rendering.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo dei flussi di lavoro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# Utilizzo dei flussi di lavoro

In Flussi di lavoro, puoi scegliere o creare predefiniti di rendering per gli output di Substance. Questi predefiniti sono reti shader per un modulo di rendering come Arnold o Vray.

>[!NOTE]
>
> **Posizioni predefinite flusso di lavoro**
> 
> **Windows**:\
> C:\Users\\Documents\maya\2022\substance\workflows\generated\
> **MacOS**:\
> /Utenti//Libreria/Preferenze/Autodesk/maya//substance/workflow/generated\
> **Linux**:\
> /home//maya//substance/workflows/generated

![](../../../assets/workflows-4.png)

Per utilizzare un flusso di lavoro, è sufficiente scegliere il predefinito dall&#39;elenco a discesa e quindi fare clic sul pulsante Crea rete shader.

![](../../../assets/workflow.gif)

## Creazione di un flusso di lavoro

Potete creare un flusso di lavoro personalizzato e aggiungerlo all’elenco Flusso di lavoro modulo di rendering. Quando si aggiunge un nuovo flusso di lavoro, tutti i nodi creati dopo il nodo Substance verranno salvati nel flusso di lavoro. Ciò consente di creare un numero qualsiasi di nodi di ombreggiatura per creare una rete shader personalizzata completa che può essere salvata come flusso di lavoro predefinito.

## ![](../../../assets/saved-workflow.png) gestione dei flussi di lavoro

### Salvataggio dei flussi di lavoro personalizzati

1. Create manualmente gli output delle Substance e collegateli a un materiale come aiStandardSurface.
   1. Per creare la rete dello shader, potete utilizzare qualsiasi nodo Maya o eseguire il rendering di nodi specifici.
1. Fai clic sul pulsante **Crea flusso di lavoro** e immetti un nome per il predefinito del flusso di lavoro.

### Duplicazione dei flussi di lavoro

È possibile duplicare un flusso di lavoro facendo clic sul pulsante **Duplica flusso di lavoro**.

### Rinomina e sovrascrivi flussi di lavoro

È possibile rinominare i flussi di lavoro esistenti e sovrascrivere i flussi di lavoro con i dati aggiornati utilizzando i pulsanti **Rinomina** e **Sovrascrivi** selezionati.

### Rimozione dei flussi di lavoro

È possibile rimuovere i flussi di lavoro esistenti utilizzando il pulsante Rimuovi flusso di lavoro.
