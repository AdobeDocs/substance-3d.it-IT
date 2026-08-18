---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-3-0-0-plus.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in 3ds Max versione 3.0.0 e successive per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3Ds Max 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 3ds Max 3.0.0+

## 3ds Max 3.0.4

<b>Aggiunto/Aggiornato:</b>

* Le icone dei plug-in Substance sono state aggiornate con le icone più recenti.
* È stato aggiunto il supporto per inviare e ricevere i predefiniti tramite il connettore nel plug-in.
* Gestione menu integrata dal parametro di notifica per sostituire l&#39;utilizzo dell&#39;interfaccia principale.

<b>Corretto:</b>

* È stato risolto il problema a causa del quale il rendering dei materiali Substance 2 poteva non riuscire in IR/Produzione con Corona quando l’editor materiale lavagna è aperto e la mappa texture Substance2 è selezionata.
* È stato risolto il problema a causa del quale gli aggiornamenti del connettore Sampler creavano nuovi nodi Substance2 anziché aggiornare quelli esistenti.
* È stato risolto un problema di arresto anomalo nel plug-in 3ds Max durante l’aggiunta di un nodo Substance2 e si è assicurato che l’utilizzo dell’importazione in batch per caricare i file .sbsar non apra più l’editor dello script.
* È stato risolto il problema a causa del quale il caricamento del plug-in 3DSMax 2025 non riusciva a causa di un file dll incompatibile quando si utilizza il programma di installazione .msi.

## 3ds Max 3.0.2

<b>Aggiunto/Aggiornato:</b>

* Gestione standardizzata delle icone nel plug-in Substance incorporando tutte le icone esistenti nei file qrc e rcc, allineandosi ai metodi preferiti di Autodesk e garantendo un caricamento coerente nel pannello grafico SBSAR.
* È stata migliorata la reattività della finestra Impostazioni Substance nel plug-in per garantire che i campi di input e le relative descrizioni si adattino correttamente durante la regolazione delle dimensioni della finestra.
* Il plug-in Substance è ora compatibile con Corona 11.

<b>Corretto:</b>

* È stato risolto un problema a causa del quale la rugosità del Colore di lucentezza e della brillantezza non si collegava automaticamente nei materiali V-Ray. Ora, entrambe le proprietà si collegheranno automaticamente quando si crea un flusso di lavoro in V-Ray e Arnold.
* È stato risolto un problema dell’interfaccia utente nel plug-in a causa del quale la regolazione dell’impostazione Limite core CPU visualizzava erroneamente i valori a due cifre se il valore salvato era a una sola cifra.
* È stato corretto un errore di rendering nella console per il plug-in 3ds Max v3.0.0 relativo alla funzione Substance compatibilità. Ora i nodi Substance creati utilizzando il menu Substance importazione batch eseguono il rendering come previsto.
