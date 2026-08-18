---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/publishing-for-mobile.html"
breadcrumb-title: ''
description: Ottimizza i materiali Substance per le piattaforme mobili in Unity regolando le impostazioni e le risoluzioni delle texture.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Publishing for Mobile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pubblicazione per dispositivi mobili
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Pubblicazione per dispositivi mobili

>[!NOTE]
>
> **Dimensioni texture sui dispositivi mobili**
> 
> La risoluzione della texture impostata in Unity Editor sarà la dimensione pubblicata nel file binario dell&#39;app. Abbassando la risoluzione del materiale della Substance si creano texture con file di dimensioni inferiori.

## Piattaforme

## Apple iOS

1. Assicurati che il modulo iOS sia scaricato per la versione Unity corrispondente.
1. In Unity, modifica la destinazione di compilazione in iOS.
1. Apri le Impostazioni del lettore e modifica il campo &quot;Identificazione - Identificativo bundle&quot; per creare un elemento più univoco. (ad esempio: com.Adobe.iosProject)
1. Creare e gestire il gioco.
1. In Xcode, fai clic sul dispositivo iOS e modifica il menu a discesa &quot;Firma - Team&quot; in ID team sviluppatori.
1. Sul dispositivo iOS, passa a &quot;Impostazioni - Generale - Gestione dispositivi&quot; e fai clic su &quot;Affidabilità&quot; sull’ID del team di sviluppatori visualizzato.
1. Eseguire nuovamente la compilazione Xcode facendo clic sul pulsante &#39;Crea ed esegui schema corrente&#39; (pulsante Riproduci).
1. Il gioco dovrebbe essere in esecuzione sul dispositivo iOS.

## Sistema operativo Android

1. Assicurati che il modulo Android sia scaricato per la versione Unity corrispondente.
1. In Unity, modifica la destinazione di compilazione in Android.
1. Apri le Impostazioni del lettore e modifica il campo &quot;Identificazione - Identificativo bundle&quot; per creare un elemento più univoco. (ad esempio: com.Adobe.androidProject)
1. Creare e gestire il gioco.
1. Il gioco dovrebbe essere in esecuzione sul dispositivo Android.
