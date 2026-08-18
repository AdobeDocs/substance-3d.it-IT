---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-1-0.html"
breadcrumb-title: ''
description: Consultate le note sulla versione per il plug-in Maya versione 2.1.0 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.1.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.1.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Maya 2.1.0

Substance nel registro delle modifiche di Maya 2.1.0

* Compatibilità garantita con Python 3
* Substance Engine aggiornate alla versione 7.2.9
* Risolto l’errore con nomi di variabili mel globali in conflitto durante l’applicazione di un flusso di lavoro
* Il flusso di lavoro Redshift imposta la fresnel su metalness
* È stato aggiunto un nuovo file plug-in, substancelink, che gestisce l’interoperabilità con altri programmi Substance e Substance Launcher.
* Se si apre Substance Source ora, il modulo di avvio Substance viene aperto nella scheda Sorgente se il plug-in substanceElink è caricato.
* Il plug-in SubstanceLink consente al modulo di avvio, quando viene aggiunta l&#39;interfaccia utente, di inviare i materiali Substance Source all&#39;integrazione Maya
* Comandi di scripting aggiunti per ottenere versioni libreria interne e per aprire il modulo di avvio di Substance alla pagina di origine
* I collegamenti del sito Web ora sono aperti su [substance3d.com](http://substance3d.com) invece di [allegorithmic.com](http://allegorithmic.com)
* Quando si apre una pagina Web, nella documentazione e nei collegamenti sorgente viene aperto il browser predefinito impostato dall’utente
* In Windows, Internet Explorer non è più aperto
* È stato aggiunto un nuovo collegamento allo scaffale e un menu al Substance share.
* Sono stati aggiunti nuovi comandi per eseguire query sulla versione e sull&#39;hash di Substance Linker.
* In Maya LT, la versione è stata rimossa dal menu delle impostazioni
* Il menu Info non è più scritto in PySide2 e Python, ma in codice nativo usando Qt. Ora è disponibile in Maya LT, dove prima non lo era.
* Il menu Informazioni contiene informazioni di diagnostica diverse; ora visualizza l&#39;hash git corrispondente alla modifica nel controllo del codice sorgente.
* La copia del menu Informazioni negli Appunti ora avrà anche questo hash git, insieme alla versione di Maya per cui è creato il plug-in.
* Le licenze nella finestra Informazioni su ora si aprono come file di testo
* Aggiunto il supporto per Maya 2017
* Il generatore di script del flusso di lavoro non genera più stringhe per il membro &#39;ordering&#39;. Tutti i flussi di lavoro esistenti verranno gestiti correttamente

Comandi di scripting aggiunti:\
substance-emaya:\
\* substanceUtilityGetLinkerVersion\
\* substanceUtilityGetLinkerHash\
\* substanceUiOpenAboutWindow\
\* substanceUiOpenSourceWebsite\
\* substanceUiOpenDocumentation\
\* substanceUiOpenShareWebsite

substanceLink:\
\* substanceLinkGetLinkVersion\
\* substanceLinkGetPortalCliVersion\
\* substanceLinkOpenLauncher

Questa versione è stata rilasciata per Maya 2017, 2018, 2019 e 2020 su Windows,\
Linux e Macos. È stato anche pubblicato per Maya LT 2018, 2019 e 2020 il\
Windows e MacOS.
