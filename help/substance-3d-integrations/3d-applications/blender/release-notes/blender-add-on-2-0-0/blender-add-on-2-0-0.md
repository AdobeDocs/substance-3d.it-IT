---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/blender/release-notes/blender-add-on-2-0-0.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il componente aggiuntivo Blender versione 2.0.0 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Componente aggiuntivo 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Componente aggiuntivo 2.0.0

Substance 3D Addon 2.0 segna un aggiornamento trasformativo per gli utenti di Blender, con un&#39;architettura plug-in completamente refactoring. Questa riprogettazione si concentra su un&#39;integrazione senza interruzioni, prestazioni migliorate e una base flessibile per le espansioni future. Rappresenta non solo un aggiornamento, ma una reimmaginazione di come i materiali Substance vengono gestiti all&#39;interno di Blender, soddisfacendo le esigenze in evoluzione dei professionisti 3D.

<b>Aspetti salienti della versione 2.0:</b>

* Architettura con refactoring: struttura di plug-in migliorata per prestazioni e integrazione migliori
* Supporto per l’espansione futura: l’aggiornamento getta le basi per l’aggiunta semplice di nuove funzioni in futuro
* Compatibilità più ampia: completamente compatibile con Blender versione 3.0 e successive, incluso il supporto per gli utenti Mac

<b>Aggiunto/Aggiornato:</b>

* [SRE] Substance Engine il supporto per la selezione (GPU è l’impostazione predefinita)
* [SRE] Nuovi formati di immagine per esportare le texture
* [SRE] Profondità di bit la selezione per ogni tipo di mappa
* [BLD] Supporto per output di valore
* [BLD] Supporto input stringa
* [SRE] È stata aggiunta l’opzione per selezionare la cartella temporanea predefinita per la destinazione di esportazione delle immagini

<b>Corretto:</b>

* [SRE] Miglioramento generale delle prestazioni
* [BLD] Problemi di comunicazione risolti tra gli strumenti di integrazione e Blender
* [BLD] Impossibile installare/avviare gli strumenti di integrazione
* [BLD] Gli strumenti di integrazione non terminano quando si chiude Blender
* [BLD] Il materiale non si aggiorna quando si modifica il tipo di file di una mappa
* [SRE] Tutte le mappe dei materiali vengono esportate in qualsiasi momento
* [SRE] Gli strumenti di integrazione esportano mappe normali con scale
* [SRE] Il caricamento della Substance non termina mai
* [SRE] Le unità Dimensioni fisiche non vengono regolate in base alla scena
* [BLD] I predefiniti generati in Blender non funzionano con altre integrazioni
* [BLD] Il materiale non si aggiorna nei cicli
* [BLD] I limiti soft e hard degli input vengono ignorati
* [BLD] L’intensità del colore non si aggiorna correttamente quando si regola un parametro
* [SRE] La disinstallazione degli strumenti di integrazione non riesce
* [SRE] È stato risolto il problema a causa del quale la duplicazione di materiali più volte causava un errore.
* [SRE] Lo spazio colore dei nodi immagine ora corrisponde correttamente alle preferenze dell&#39;utente.

<b>Problemi noti:</b>

* Quando si utilizza Blender v4.0+, i socket non sono in ordine dopo aver attivato e disattivato più volte
* Cltr+Z per annullare le modifiche potrebbe causare errori
* Il caricamento di un file vuoto o di una cartella invece di un file .sbsar potrebbe interrompere il plug-in
* Supporto per la modalità headless di Blender
