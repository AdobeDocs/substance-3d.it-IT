---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-5.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.4.5 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.4.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Unità 2.4.5

Rilasciato il 6 aprile 2020

* Aggiunto: controllo delle risorse HDRP utilizzando l’API 2019.3
* Aggiunto: aggiornamento a Substance Engine 7.2: corregge alcuni materiali Substance da Source che non funzionano
* Aggiunto: aggiornare le impostazioni di destinazione in base alla risoluzione della CPU
* Aggiunto: Impostazione risoluzione massima motore CPU (impostazione 4k o 2k)
* Aggiunto: convertire Substance non HDRP in un progetto HDRP
* Fisso: Arresto anomalo durante l’importazione di grandi quantità di Substance
* Corretto: eccezione quando si fa clic su reimporta in modalità di riproduzione dopo aver modificato i parametri di Substance
* Fisso: convalida della risoluzione di output (texture) ( API per limitare il motore CPU a 2 KB) Preferenza utente per impostare il valore predefinito su 4K
* Corretto: se si fa clic su &quot;Genera mappe mappa mappa&quot; in un grafico a Substance in modalità di riproduzione, la modifica dei parametri provoca un blocco infinito
* Corretto: durante l’utilizzo del plug-in Substance in un progetto HDRP, l’utilizzo della compressione Nessuna imposta le texture in scala di grigi sull’Alpha 8
* Corretto: GameObject deselezionato in modalità di riproduzione
* Fisso: la mappa di rugosità non viene aggiornata con la modifica del parametro
* Corretto: l’output della maschera non viene generato correttamente per alcuni file di Substance in HDRP
* Corretto: arresto anomalo durante il passaggio dal menu a discesa della mappa alfa compressa tra due opzioni
* Corretto: la casella di controllo dell&#39;istanza GPU viene ripristinata quando si fa clic all&#39;esterno del materiale della Substance.
* Fisso: quando si utilizza la funzione Duplicate(), il grafico della Substance duplicato non dispone dello smoothness inserito correttamente nell&#39;alfa del metallizzato.
* Corretto: se si cambia la destinazione di creazione in Android, le texture risultano nel formato errato fino a quando non vengono reimportate manualmente.
* Corretto: l&#39;eliminazione di un file di Substance in Unity causerà un NullReferenceException.
* Corretto: disabilitare l’uso delle API HDRP di Unity 2019.3 per le versioni precedenti

Problemi noti:

* La casella di controllo delle emissioni non è attivata per impostazione predefinita e il valore HDR viene impostato su nero durante l’importazione di una Substance.
* Le proprietà dei materiali provenienti da colli con materiali standard per le sostanze non vengono riportate all’importazione.
* L&#39;aggiornamento da 2017-2019/2020 non funziona in HDRP
* Se si fa clic sull’opzione di blocco 2048 nel menu delle impostazioni mentre è selezionato 4096 nelle impostazioni di destinazione (senza fare clic su applica), si verifica un errore nel registro della console
