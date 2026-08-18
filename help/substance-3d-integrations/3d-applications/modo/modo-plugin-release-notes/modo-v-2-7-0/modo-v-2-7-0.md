---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/modo/modo-plugin-release-notes/modo-v-2-7-0.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in MODO versione 2.7.0 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Plugin Release Notes > Modo v. 2.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modo v. 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# Modo v. 2.7.0

* Numerose correzioni agli arresti anomali
* Supporto float a 32 bit
* Texture 4k nel motore CPU e texture 8k nel motore GPU
* nuovo formato LPK per la versione del plug-in
* nuovo menu Kit per il plug-in Substance
* glTF / Supporto dello shader basato su principi per MODO 12.0
* È stato aggiunto il percorso relativo per i file Substance.
* Supporto Linux
* Nuova interfaccia utente per il caricamento e il salvataggio dei predefiniti
* I predefiniti incorporati vengono caricati da Designer
* Finestra di avviso Memoria GPU rimossa
* Comandi di caricamento/salvataggio predefiniti modificati

  I nuovi comandi disponibili sono:

  **substance.getsbsname** Convertire l&#39;identificatore di un oggetto substance nel nome interno

  Tutti questi si aspettano un nome interno appropriato acquisito da substance.getsbsname:

  **substance.setpreset** Imposta il predefinito corrente di una Substance sull&#39;indice **substance.getpresetindex** Ottiene l&#39;indice del predefinito corrente **substance.getpresetat** Restituisce il nome della stringa di un predefinito in un dato **index substance.getpresetcount** Restituisce il numero di predefiniti di una Substance **substance.savepresetfile** Salva un predefinito della configurazione corrente nel percorso del file specificato **substance.loadpresetfile** Carica un file del predefinito nella Substance specificata da un percorso di file

  Comandi dell&#39;interfaccia utente:

  Comando dell&#39;interfaccia utente **substance.loadpresetui** per il caricamento di un predefinito **substance.savepresetui** Comando dell&#39;interfaccia utente per il salvataggio di un predefinito **substance.selectpresetui** Comando dell&#39;interfaccia utente per l&#39;impostazione del predefinito
