---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/installing-to-source-builds-ue5.html"
breadcrumb-title: ''
description: Installa il plug-in Substance 3D nelle build sorgente di Unreal Engine 5 per modifiche personalizzate al motore.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Installazione nelle compilazioni sorgente - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# Installazione nelle compilazioni sorgente - UE5

Il plug-in Substance può essere utilizzato con le versioni di Unreal Engine create dalla fonte. A tale scopo, il plug-in può essere installato in una cartella C++project o nella cartella engine di una build di origine.

>[!NOTE]
>
> Questi metodi richiedono che sia scaricata una versione del plug-in dal marketplace. La cartella dei plug-in Substance può essere trasferita tra computer e build UE.

## Installazione in una cartella di progetto C++

1. Nella cartella del progetto, crea una cartella Plug-in, se non esiste già.
1. All’interno della cartella Plugin, crea una cartella Runtime.
1. Posiziona la cartella Substance all&#39;interno della cartella Runtime. UTENTI LINUX: dopo il passaggio 3, individuare la cartella &quot;include&quot; nella cartella Substance e rinominarla in maiuscolo con la &quot;i&quot; (include > Include).
1. Avvia Unreal Engine.
1. Apri il progetto C++ tramite il modulo di avvio.
1. Dopo aver avviato il progetto, Unreal Engine chiederà se desideri ricompilare i componenti del plug-in prima di avviarlo, seleziona sì. Questa operazione verrà eseguita tramite Microsoft Visual Studio (Windows, Linux) o Xcode (Mac).
1. Unreal Engine verrà chiuso, ma i componenti verranno costruiti in background. Questo processo può richiedere circa 5 minuti. Al termine, il progetto si aprirà. Se l&#39;operazione non riesce, viene visualizzata una finestra di errore.

## Installazione nella cartella del motore

>[!NOTE]
>
> Per poter installare il plug-in nella cartella Engine, è necessario eseguire i passaggi precedenti per ricreare la cartella dei file binari del plug-in.

1. Copia la cartella Substance dalla cartella del progetto > Plug-in > Runtime.
1. Apri la cartella Versione motore originale e seleziona Motore > Plug-in > Marketplace.
1. Incolla la cartella Substance.
1. Apri l’editor del motore originale. Se necessario, create un nuovo progetto.
1. Apri il menu Plug-in e verifica che l’opzione Substance plug-in sia abilitata.
