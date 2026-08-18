---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/substance-in-maya-overview.html"
breadcrumb-title: ''
description: Scopri il plug-in Substance per Maya e come importare e utilizzare i materiali Substance nel tuo flusso di lavoro.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance in Maya Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panoramica di Substance in Maya
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Panoramica di Substance in Maya

## Panoramica del plug-in

Il plug-in Substance consente di caricare il materiale della Substance creato nel Substance Designer direttamente in Maya. Il plug-in creerà un materiale Maya e immetterà le texture della sostanza negli input dei canali dei materiali. Potete quindi apportare modifiche ai parametri della sostanza e le texture verranno aggiornate automaticamente.

>[!NOTE]
>
> Assicurati che il plug-in sia caricato in Impostazioni/Preferenze ->Gestione dei plug-in Maya

![](https://helpx-prod.scene7.com/is/image/HelpxProd/plugin-4?$png$&jpegSize=100&wid=618)

## Apertura di una Substance

1. Apri Hypershade e nell’Editor nodi fai clic con il pulsante destro del mouse e scorri verso l’alto nel menu di marcatura per scegliere Crea nodo. Viene aperta la finestra Crea nodo. Da qui, è possibile cercare il nodo Substance.

   ![](../../../assets/createnode.png)

   Puoi anche premere TAB nell’editor dei nodi e nel campo di testo, digita substance per filtrare in base alle opzioni substance. Dalle opzioni, scegliete Substance texture.
1. Selezionare il nodo Substance e nell&#39;Editor proprietà e sfogliare per caricare un file di Substance (.sbsar).

   ![](../../../assets/1.png)
1. Il menu a discesa Grafico selezionato verrà compilato se la Substance contiene più grafici. Il grafico scelto verrà utilizzato per creare il materiale.
1. Il pulsante Informazioni grafico consente di visualizzare gli attributi del grafico impostati in Substance Designer.
1. Impostate la Risoluzione scegliendo un valore dalla casella a discesa Larghezza e Height. Blocca rapporto è attivato per impostazione predefinita.
1. Attivate Cache Outputs to Disk per eseguire il baking degli output della Substance su disco in modo che possano essere utilizzati con renderer come Arnold. Il file memorizzato nella cache verrà riletto dal plug-in utilizzando un nodo di file Maya.

   ![](../../../assets/outputsettings.png)
1. Scegliete un flusso di lavoro per il modulo di rendering in uso e fate clic sul pulsante Crea rete shader. Viene creata una rete di shader per il flusso di lavoro del modulo di rendering. Ora puoi applicare il materiale nella scena.

   ![](../../../assets/createnetwork.gif){width="1000px"}
