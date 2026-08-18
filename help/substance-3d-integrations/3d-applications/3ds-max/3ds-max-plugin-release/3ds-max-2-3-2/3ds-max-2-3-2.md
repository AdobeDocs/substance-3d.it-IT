---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-2.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in 3ds Max versione 2.3.2 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 3ds Max 2.3.2

Rilasciato l’8 aprile 2020

Oggi abbiamo rilasciato la versione 2.3.2 del plug-in, che è per la maggior parte una versione bug fix in aggiunta alla versione 2.3.1.

2.3.2 Versione:

* Substance Engine aggiornate alla versione 7.2.9
* Risolto il problema relativo all’arresto anomalo di Redshift/VRay in 3ds Max 2018, 2019 e 2020
* Gli errori di asserzione di debug non verranno più visualizzati
* Il nodo Substance2 dispone ora correttamente delle interfacce di script per iMultipleOutputChannelsWithValues
* La voce Substance sorgente nel menu aprirà il modulo di avvio Substance nella scheda Sorgente, se è installato
* I materiali Substance ora dovrebbero essere aggiornati correttamente quando si lavora con il modulo di rendering Corona
* Gli output della Substance non vengono più sostituiti temporaneamente con le immagini se utilizzati con VRay Next
* Finestra di dialogo di compatibilità del rendering rimossa dalla visualizzazione automatica. Se necessario, è ancora disponibile nella finestra di dialogo delle impostazioni
* È stato risolto un possibile problema relativo all’esportazione di un file fbx mentre il materiale Substance veniva applicato in 3ds Max 2021.

Problemi noti:

* In 3ds Max 2018, l’esportazione di un file fbx con un materiale Substance collegato all’oggetto si arresta in modo anomalo nel plug-in fbxmax.dlu. Stiamo attualmente parlando con Autodesk per verificare se è possibile eseguire alcune operazioni o se si tratta di una limitazione della versione precedente dell&#39;integrazione fbx. La soluzione precedente non era affidabile ed è stata rimossa. Questo non si verifica in 3ds Max 2019 o versioni successive.

Questa versione è stata rilasciata per 3ds Max 2018, 2019, 2020 e 2021.
