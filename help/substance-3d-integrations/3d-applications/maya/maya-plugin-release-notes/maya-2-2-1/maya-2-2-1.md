---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-2-1.html"
breadcrumb-title: ''
description: Consultate le note sulla versione per il plug-in Maya versione 2.2.1 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.2.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.2.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Maya 2.2.1

Versione di Maya 2.2.1:

* Aggiorna Substance Engine alla versione 8.3.0
* Aggiungere il supporto nativo per Arnold, eliminando la necessità di cache su disco
* Questo può essere utilizzato dopo aver attivato le estensioni di rendering nelle impostazioni e riavviato Maya
* Le versioni supportate sono:
* Maya 2017 - MtoA 3.1.0/Arnold 5.2.0
* Maya 2018 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0
* Maya 2019 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2020 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2022 - MtoA 4.2.1/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Directory di installazione aggiornata in Windows e MacOS
* I file binari in MacOS/Windows sono ora firmati utilizzando i certificati di Adobe
* Gli interruttori dei canali sono ora nascosti quando l&#39;autore della barra laterale è Allegorithmic o Adobe, invece di Allegorithmic
* Aggiunta di una nuova interfaccia utente del flusso di lavoro, con funzionalità aggiuntive per duplicare, sovrascrivere, rinominare ed eliminare i flussi di lavoro

Sono stati aggiunti i seguenti nuovi comandi di scripting:

substanceEmaya

substanceGetEnableRenderingExtensions

substanceSetEnableRenderingExtensions

substanceworkflow.py

substanceWorkflowIsReadOnly

substanceWorkflowRenameWorkflow

substanceWorkflowDuplicateWorkflow

substanceWorkflowOverwriteWorkflow

substanceWorkflowRemoveWorkflow

Correzioni di bug:

* Correzione dell’errore all’apertura della finestra di dialogo Impostazioni
* Le funzioni del flusso di lavoro non hanno più esito negativo quando è stato generato un pyc

Questa versione è rilasciata per Maya 2017, 2018, 2019, 2020 e 2022 su Linux, MacOS e Windows e per Maya LT 2018, 2019 e 2020 su MacOS e Windows
