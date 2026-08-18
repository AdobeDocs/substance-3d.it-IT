---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-7-0.html"
breadcrumb-title: ''
description: Consultate le note sulla versione per il plug-in 3ds Max versione 2.7.0 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 3ds Max 2.7.0

<b>Aggiunto/Aggiornato:</b>

* Il motore di Substance è stato aggiornato alla versione 9 nel plug-in 3ds Max, migliorando le prestazioni e la compatibilità.

<b>Corretto:</b>

* È stato risolto un problema di arresto anomalo nelle versioni 2019, 2022, 2023 e 2024 di 3ds Max, a causa del quale il trascinamento di un nodo Substance 2 nell’editor materiale di Slate causava l’arresto anomalo del programma. Il nodo Substance 2 può ora essere trascinato e rilasciato nell&#39;editor materiale di ardesia.
* È stato risolto un problema nel plug-in Substance per 3ds Max, a causa del quale la selezione di &quot;Substance ad Arnold&quot; e altri flussi di lavoro non creava nodi pertinenti nell&#39;editor di slate di materiali, ma apriva erroneamente un Maxscript con un errore di compilazione. I nodi per i flussi di lavoro come Arnold ora vengono generati correttamente e collegati automaticamente.
* È stato risolto un problema a causa del quale l’esportazione di risorse di partenza/predefiniti (.sbsar - mappa texture Substance2) da Substance 3D Sampler e la loro conversione nel modulo di rendering Corona (versioni da 6 a 9hf1) in 3ds Max causava materiali danneggiati, il rendering con colore di base nero e normali di rilievo danneggiati. Inoltre, questo aggiornamento risolve l&#39;inaccessibilità della scheda delle proprietà della Substance nei materiali, un problema che influenzava anche le conversioni in Vray.
* È stato risolto un problema nel plug-in 3ds Max a causa del quale il collegamento o lo scollegamento degli input dalle texture Substance2 a Corona Material causava arresti anomali.
* È stato risolto il problema di compatibilità in 3ds Max 2024 in cui gli script Python incorporati o chiamati in un file MaxScript non erano consentiti per impostazione predefinita.
* È stato risolto un problema nel plug-in 3Ds Max a causa del quale l’importazione e l’esecuzione del plug-in Substance in Corona causavano la visualizzazione di materiali neri e lucidi nelle anteprime dello shader e nei rendering. Questo problema è stato risolto con successo, garantendo la corretta visualizzazione e il rendering delle mappe Substance con il modulo di rendering Corona.

Questa versione è disponibile per 3ds Max 2021, 2022 e 2023
