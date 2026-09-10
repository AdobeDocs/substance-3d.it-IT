---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-1.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.5.1 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.5.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Unità 2.5.1

Rilasciato il 21 maggio 2020

Aggiunto

* Supporto della pipeline di rendering universale: la texture Substance utilizzerà automaticamente gli shader e i materiali URP

Fisso

* Substance impostazione risoluzione massima motore CPU:
  * Il nome del campo nel menu Substance impostazioni è stato aggiornato da &quot;Blocco texture \*\*&quot; a &quot;Risoluzione massima motore CPU Substance&quot;
  * Verrà visualizzata una notifica di avvertenza che indica che tutti i materiali Substance verranno reimportati quando l&#39;impostazione viene modificata
* È stato rimosso il messaggio di debug non necessario visualizzato al momento dell&#39;installazione (&quot;TextureClamp = 4096 Unity.Engine.Debug:Log(Object)&quot;)
* Progetto HDRP: le proprietà dei materiali presenti sia nei materiali standard che nei materiali HDRP vengono trasferite quando si importano pacchetti che includono Substance
* Le maschere Riflessione e HDRP vengono create e funzionano come previsto quando viene importato un materiale Substance da un pacchetto Substance della precedente versione di Unity
* Il materiale duplicato della Substance sarà il colore desiderato e non più giallo quando si utilizza la funzione di duplicazione
* L&#39;origine Substance verrà caricata come previsto dopo la chiusura e la riapertura di Unity
* Arresti anomali durante l’importazione di un pacchetto in un progetto HDRP (in modo intermittente)
* Il cursore funziona come previsto per i materiali Substance con un parametro esposto in cui l’editor è impostato su Colore (scala di grigi)
* Arresto anomalo quando si fa clic su &quot;Ripristina predefinito&quot; con Substance grafici che non hanno una risoluzione predefinita
* Arresto anomalo quando si modifica la dimensione di output di un materiale Substance quando il parametro della dimensione di output non è esposto
* La creazione per iOS non avrà esito negativo
* Gli script che utilizzano i materiali Substance verranno eseguiti durante la creazione per Windows Standalone
