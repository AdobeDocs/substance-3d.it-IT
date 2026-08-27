---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-2.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.5.2 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.5.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Unità 2.5.2

Rilasciato il 23 luglio 2020

Aggiunto:

* Funzione &quot;IsProcessing()&quot; che indica se il modulo di rendering è occupato o inattivo (non occupato)

Fisso:

* Non viene più visualizzato un errore durante l&#39;impostazione delle impostazioni di destinazione 2048 clamp e 4096
* Le proprietà dei materiali verranno trasferite quando si esegue l&#39;aggiornamento a HDRP e/o URP da Standard
* Gli script che modificano il materiale Substance funzioneranno come previsto quando vengono distribuiti su dispositivi mobili
* Canale rosso non viene più copiato in Alpha e l’Alpha predefinito viene impostato su Bianco
* Arresto anomalo sulla modifica delle impostazioni di destinazione in Mac
* Errore NullReferenceException rimosso durante la creazione del materiale Unity
* Errore rimosso quando si esce dalla modalità di riproduzione dopo aver modificato le proprietà dell’Affiancamento
* Attivare l’istanza GPU
* I materiali che utilizzano la trasparenza non scompariranno o diventeranno neri in modo errato quando è attiva la modalità di riproduzione
* I materiali Substance non verranno distrutti nel progetto HDRP durante l&#39;aggiornamento del plug-in
