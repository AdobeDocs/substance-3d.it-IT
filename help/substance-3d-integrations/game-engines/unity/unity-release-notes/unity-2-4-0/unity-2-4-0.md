---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-0.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.4.0 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.4.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Unità 2.4.0

>[!WARNING]
>
> Unity ha modificato l&#39;architettura di compilazione predefinita in x86 invece di x86\_64.\
> Gli script non verranno eseguiti se fanno riferimento a Substance. Dovrai tornare a x86\_64 e la build funzionerà.

## Nuove funzioni:

* Supporto progetto HDRP aggiunto (anteprima)
* Preferenze aggiunte nel menu Substance
* È stata aggiunta la possibilità di impostare le impostazioni di importazione predefinite per la risoluzione delle Substance.
* È stata aggiunta la possibilità di impostare la compressione Normale predefinita.
* È stata aggiunta la possibilità di generare tutti gli output durante l’importazione di una Substance.
* Supporto per output e output personalizzati con lo stesso utilizzo
* Impostazioni di Risoluzione piattaforma aggiunte
* Sono stati aggiunti bug di supporto IL2CPP

### Correzioni di bug:

* È stato corretto un bug a causa del quale l’apertura della Substance Source nel sistema operativo Mac generava un errore Linux.
* Riduzione del tempo necessario per cambiare piattaforma. La conversione delle texture per le piattaforme mobili viene ora eseguita in fase di creazione anziché quando si cambia piattaforma di destinazione.
* Errore di asserzione non riuscita durante l&#39;importazione di sbsar
* L&#39;aggiornamento dei progetti tramite .NET 3.5 causa la rottura dei materiali Substance
* Origine Substance non supportata nella finestra di dialogo linux visualizzata su OS X
* La modifica del nome del grafico distrugge prefabbricati e file di scena nella modalità di serializzazione ForceText
* Substance materiali con più output utilizzando lo stesso utilizzo interromperà Plugin non supporta output personalizzati in sbsar

### Problemi noti:

* Quando si aggiorna un progetto da 2017-2018/2019, dopo che l&#39;utente ha importato il plug-in Substance, Unity deve essere riavviato per consentire l&#39;aggiornamento del progetto.\
  Soluzione alternativa: crea un pacchetto di risorse/progetto e importa tale pacchetto in un progetto più recente con il plug-in 2.4.0. I file di Substance devono essere convertiti correttamente.
* Unity ha modificato l&#39;architettura di compilazione predefinita in x86. Attualmente, il plug-in Substance supporta solo x86\_64.

**Non Più Completamente Supportato:**

* Substance Live Link è stato rimosso dal pacchetto Asset Store. (Il pacchetto può ancora essere scaricato da Substance share)
