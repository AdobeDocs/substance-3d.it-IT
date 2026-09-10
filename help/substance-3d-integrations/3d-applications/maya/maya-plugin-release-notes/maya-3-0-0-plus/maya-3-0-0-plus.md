---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-3-0-0-plus.html"
breadcrumb-title: ''
description: Consultate le note sulla versione per il plug-in Maya versione 3.0.0 e successive per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > Maya 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Maya 3.0.0+

## Maya 3.0.3

<b>Aggiunto/Aggiornato:</b>

* È stato migliorato il sistema di memorizzazione nella cache del plug-in Maya in modo che venga memorizzato nella cache una sola volta al momento della creazione iniziale della rete, con il ricaching manuale abilitato.
* È stata fornita un’opzione per modificare la posizione della cartella &quot;substance&quot; nel plug-in Maya.
* È stato aggiornato il sistema di importazione del flusso di lavoro del plug-in Maya per garantire la compatibilità con l’aggiornamento di Autodesk alla versione 3.12 di Python.
* Le icone dei plug-in Substance sono state aggiornate con le icone più recenti.
* È stato aggiunto il supporto per inviare e ricevere i predefiniti tramite il connettore nel plug-in.

<b>Corretto:</b>

* Risolto il problema per cui il caricamento/scaricamento del plug-in Substance per Maya genera una schermata di errore e arresti anomali.
* Sono stati risolti problemi di memorizzazione nella cache, per garantire in particolare che i file .exr facciano riferimento correttamente e ridurre i blocchi relativi alla memorizzazione nella cache in scene di grandi dimensioni.
* È stato risolto il problema a causa del quale l’anteprima del materiale nella finestra di esempio non veniva visualizzata quando un file SBSAR veniva caricato nel plug-in Maya.
* È stato risolto il problema a causa del quale il connettore non riceveva il file SBSAR se almeno un file SBSAR era già in Hypershade.
