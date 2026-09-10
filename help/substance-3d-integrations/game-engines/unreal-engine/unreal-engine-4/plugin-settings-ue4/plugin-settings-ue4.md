---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/plugin-settings-ue4.html"
breadcrumb-title: ''
description: Configura le impostazioni Substance plug-in in Unreal Engine 4 tramite le Impostazioni del progetto per personalizzare il comportamento dei plug-in.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Plugin Settings - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Impostazioni plug-in - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---


# Impostazioni plug-in - UE4

Per accedere alle impostazioni, seleziona Modifica > Impostazioni progetto, scorri verso il basso fino alla categoria Plug-in e fai clic su Substance.

![](../../../../assets/settings-36.png){width="400px"}

## Budget hardware

Il budget di memoria è la quantità massima di memoria da utilizzare per il motore della sostanza. Può essere aumentato per migliorare la velocità di elaborazione delle sostanze, ma consumerà più risorse di sistema. (Non sempre un aumento utile a livello di progetto).

Core CPU indica il numero di core che il motore di Substance è autorizzato a utilizzare. Questo include sia core fisici che thread hyper. Se il numero assegnato è maggiore dei core disponibili in un sistema, per impostazione predefinita verranno utilizzati tutti i core disponibili.

## Cucinare

Il conteggio dei livelli di punta rimosso durante la cottura cambia il modo in cui vengono create le texture per un pacchetto. Questa impostazione può migliorare notevolmente i tempi di caricamento e ridurre le dimensioni del pacchetto perché i livelli di texture mip più grandi non dovranno più essere caricati. I LOD più piccoli/con risoluzione più bassa verranno caricati e quelli più alti verranno impostati automaticamente da UE4. Le sostanze vengono poi trattate attraverso il motore delle sostanze e aggiornate in fase di esecuzione con i LOD ad alta risoluzione.

La Substance Engine può essere CPU o GPU. Il motore GPU consentirà di creare texture 4K. Il motore della CPU è limitato a 2K.

## Generazione predefinita:

La modalità di generazione della Substance (SGM) controlla la modalità di generazione delle texture. Questa è un&#39;impostazione globale per la Substance. L&#39;SGM può essere modificato per Substance in fabbrica.

**SGM Eseguito i baking**: Esegue i baking le texture Substance. Perdita della capacità di modificare i parametri in fase di runtime.

**SGM durante il caricamento della sincronizzazione**: blocca l&#39;applicazione durante il caricamento delle Substance.

**SGM in Load Sync e Cache**: memorizza nella cache un risultato intermedio della texture sul disco.

**SGM in modalità di caricamento asincrono**: non bloccante. Le Substance vengono generate in background.

**SGM su Async Load e Cache**: memorizza nella cache un risultato intermedio della texture sul disco.

***Il valore predefinito della piattaforma è Load Async and Cache***

## Substance Factory

Per modificare l&#39;SGM per una Substance, fare clic con il pulsante destro del mouse sulla Substance Factory>Azioni risorse>Modifica in blocco tramite matrice proprietà. È quindi possibile modificare l&#39;SGM.

![](../../../../assets/sgm.png){width="800px"}

## Ottimizzazione:

Questo limita il numero di sostanze asincrone che possono essere trasferite al motore delle sostanze per ogni lotto. Numeri più bassi velocizzano il completamento e l&#39;aggiornamento di un&#39;attività asincrona in cui numeri più alti eseguono il rendering in batch ed elaborano più sostanze alla volta. (Più alto è il numero, più gli aggiornamenti delle texture risultano discontinui perché il tempo che intercorre tra un aggiornamento e l’altro è maggiore).

## Rendering asincrono/sincrono

Il rendering della sincronizzazione è una chiamata di rendering bloccante. Questo passerà un&#39;istanza del grafico della sostanza al motore della sostanza da ricalcolare, ma interromperà l&#39;esecuzione fino a quando il motore della sostanza non avrà terminato l&#39;elaborazione della sostanza prima di continuare con qualsiasi ulteriore esecuzione del codice. Il risultato verrà inoltre aggiornato sullo schermo al termine del processo.

Async aggiungerà il tuo grafico a una coda e invierà più grafici al motore substance alla volta (impostato da impostazioni substance) all&#39;interno dell&#39;aggiornamento del plug-in. A differenza del rendering della sincronizzazione, non appena vengono inviati via, il programma continua a funzionare come al solito invece di aspettare che il motore substance sia completo. Quando il motore della sostanza ha finito quel batch, invia i risultati indietro, li applichiamo agli output, e diamo il via a un altro batch.
