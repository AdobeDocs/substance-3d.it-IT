---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/upgrading-projects-known-issues.html"
breadcrumb-title: ''
description: Informazioni sull'aggiornamento dei progetti Unity con materiali Substance e problemi noti da evitare durante la migrazione.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Upgrading ProjectsKnown Issues
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aggiornamento dei progettiProblemi noti
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# Aggiornamento dei progetti/Problemi noti

>[!WARNING]
>
> Il plug-in Substance 3D per Unity 3.0.0 non supporta la compatibilità con le versioni precedenti. Pertanto, assicurati di utilizzare Unity 2020.3.27x e versioni successive.
> 
> Unity ha modificato l&#39;architettura di compilazione predefinita in x86 invece di x86\_64.\
> Gli script non verranno eseguiti se fanno riferimento a Substance. Dovrai tornare a x86\_64 e la build funzionerà.

## Problemi noti

* Errore &quot;*Asserzione non riuscita sull&#39;espressione&quot; durante l&#39;esplorazione delle cartelle del pannello.*
  * Si tratta di un errore che si verifica alla fine dell&#39;unità quando vengono apportate modifiche all&#39;interfaccia utente, in genere modifiche di miniature, dovrebbero essere un messaggio innocuo.
* *Gli input dell&#39;immagine sembrano essere bloccati a 8 bit*
  * Questo problema è stato risolto nella versione 3.8.0-3. Il flusso di lavoro corretto consisterebbe nel modificare il formato predefinito di Unity per la texture in RGBA64. Il plug-in si occuperà di inviare correttamente tali informazioni a Substance Engine.
