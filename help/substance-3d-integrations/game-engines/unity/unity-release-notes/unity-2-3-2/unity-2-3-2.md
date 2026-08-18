---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-2.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.3.2 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Unità 2.3.2

## Nuove funzioni:

* Serializzazione dei materiali
* Riflesso: il plug-in ora consente l&#39;importazione di vecchi file di Substance in pacchetti (aggiornati automaticamente ai nuovi dati di Substance all&#39;importazione)
* Le proprietà dei materiali sono riportate all&#39;importazione di colli con dati di Substance
  * Nota: applicabile solo ai pacchetti creati con l&#39;aggiornamento 2.3.0 o versioni successive
* È stato aggiunto il pulsante Texture forno al menu Substance grafico

### Correzioni di bug:

* È stato risolto un problema a causa del quale la suddivisione in porzioni del materiale della Substance veniva ripristinata se la cartella Libreria veniva rimossa.
* Velocità migliorata in uscita dalla modalità di riproduzione
* È stato risolto un arresto anomalo durante l’aggiornamento del plug-in mentre era in uso la DLL di Substance.
* La cartella Allegorithmic ora non può essere eliminata in Unity.
  * Nota: il contenuto della cartella Allegorithmic non può essere modificato. La sua eliminazione all&#39;interno di Unity può causare diversi problemi, facendo sì che la cartella Allegorithmic riappaia magicamente quando Unity viene chiusa e riaperta. Ora viene visualizzato un avviso che informa l&#39;utente di eliminarlo con Unity chiuso manualmente dalla cartella Risorse del progetto
* Velocità migliorata in uscita dalla modalità di riproduzione
* È stato corretto un bug che reimpostava le proprietà del materiale della Substance quando la cartella Libreria veniva rimossa.

## Problemi noti:

**Plug-in Substance principale**

* L&#39;utente deve disabilitare &quot;Abilita codice di bit&quot; nel menu Impostazioni di compilazione in Xcode per generare per iOS
* La Substance non funziona con Bundle risorse
* Le icone di anteprima della Substance nel Browser risorse vengono tutte modificate nell&#39;icona Substance S dopo una reimportazione

**Scripting**

* Lo scripting non funziona in fase di runtime se il progetto è impostato su x86 nelle impostazioni di compilazione
* Problemi con l’utilizzo del back-end di scripting il2cpp con determinate piattaforme di compilazione

**Substance Painter collegamento dinamico**

* La creazione di un progetto dopo aver colorato con Substance Live Link riporterà la trama dipinta a un materiale predefinito
* Canale AO non inviato con Painter Live Link
* Le trame con più materiali non funzionano in Unity Live Link
* Il modo in cui Unity LiveLink utilizza SimpleJson si scontra con altre istanze di SimpleJson in un progetto
