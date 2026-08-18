---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/troubleshooting.html"
breadcrumb-title: ''
description: Diagnostica e risolvi i problemi con il plug-in Substance in 3ds Max utilizzando il listener di script per i messaggi di errore.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Risoluzione dei problemi
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---


# Risoluzione dei problemi

Il listener di scripting può essere utilizzato per diagnosticare gli errori rilevati durante l&#39;utilizzo del plug-in. Per aprire il listener di script, selezionate Menu script > Listener di script. Quando si verifica un errore durante l&#39;utilizzo del plug-in, nella finestra del listener di script viene visualizzato un messaggio di errore corrispondente. Per ulteriori informazioni, visitare la [documentazione ufficiale di Script Editor](https://help.autodesk.com/view/3DSMAX/2023/ENU/?guid=GUID-C8019A8A-207F-48A0-985E-18D47FAD8F36).

Per segnalare un bug, partecipa al canale #3dsmax-plugin sul [server Discord Substance](https://discord.com/invite/substance3d) o visita le [community di Adobe](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax). Le informazioni pertinenti dal registro della console e le eventuali fasi di riproduzione per il problema possono essere incluse nei report.

## Problemi noti

* *Sostituzione di un file .sbsar che utilizza un output diffuso con un file .sbsar che non utilizza un file diffuso porta al rendering nero a causa della disconnessione del file diffuso mancante.*
  * Questo è il comportamento previsto per i nodi con più output. Anziché caricare i file con estensione sbsars utilizzando lo stesso nodo, si consiglia di utilizzare nodi Substance diversi per ciascuno di essi.
