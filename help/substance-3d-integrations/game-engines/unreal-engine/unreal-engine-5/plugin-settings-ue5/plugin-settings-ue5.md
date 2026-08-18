---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/plugin-settings-ue5.html"
breadcrumb-title: ''
description: Configura le impostazioni Substance plug-in in Unreal Engine 5 tramite le Impostazioni del progetto per personalizzare il comportamento dei plug-in.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Plugin Settings - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Impostazioni plug-in - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# Impostazioni plug-in - UE5

Per accedere alle impostazioni, seleziona Modifica > Impostazioni progetto, scorri verso il basso fino alla categoria Plug-in e fai clic su Substance.

![](../../../../assets/screen-shot-2022-03-31-at-5-50-29-pm.png)

## Budget hardware

Il budget di memoria è la quantità massima di memoria da utilizzare per il motore di Substance. Può essere aumentata per migliorare la velocità di elaborazione della Substance ma consumerà più risorse. (Non sempre un aumento utile a livello di progetto).

Core CPU determina il numero di core consentiti al motore di Substance. Questo include sia core fisici che thread hyper. Se il numero assegnato è maggiore dei core disponibili in un sistema, per impostazione predefinita verranno utilizzati tutti i core disponibili.

## Cucinare

Il conteggio dei livelli di punta rimosso durante la cottura cambia il modo in cui vengono create le texture per un pacchetto. Questa impostazione può migliorare notevolmente i tempi di caricamento e ridurre le dimensioni del pacchetto perché i livelli di texture mip più grandi non dovranno più essere caricati. I LOD più piccoli/con risoluzione inferiore verranno caricati e quelli più alti verranno impostati in modo predefinito da UE5. Le Substance vengono quindi elaborate tramite il motore di Substance e aggiornate in fase di runtime con i LOD ad alta risoluzione.

La Substance Engine può essere CPU o GPU. Il motore GPU consentirà di creare texture 4K. Il motore della CPU è limitato a 2K.

## Ottimizzazione:

Questo limita il numero di sostanze asincrone che possono essere trasferite al motore delle sostanze per ogni lotto. Numeri più bassi velocizzano il completamento e l’aggiornamento di un’attività asincrona in cui numeri più alti eseguono il rendering in batch ed elaborano più Substance alla volta. (Più alto è il numero, più gli aggiornamenti delle texture risultano discontinui perché il tempo che intercorre tra un aggiornamento e l’altro è maggiore).

## Rendering asincrono/sincrono

Il rendering della sincronizzazione è una chiamata di rendering bloccante. In questo modo un&#39;istanza del grafico a Substance verrà passata al motore di Substance per essere ricalcolata, ma l&#39;esecuzione verrà interrotta fino al termine dell&#39;elaborazione della Substance da parte del motore di Substance prima di continuare con qualsiasi ulteriore esecuzione del codice. Il risultato verrà inoltre aggiornato sullo schermo al termine del processo.

Async aggiungerà il grafico a una coda e invierà più grafici al motore di Substance alla volta (impostato dalle impostazioni di Substance) nell&#39;aggiornamento del plug-in. A differenza del rendering della sincronizzazione, non appena vengono inviati fuori, il programma continua a funzionare come al solito anziché attendere il completamento del motore di Substance. Quando il motore di Substance ha finito quel batch, invia i risultati indietro, li applichiamo agli output, e avviamo un altro batch.
