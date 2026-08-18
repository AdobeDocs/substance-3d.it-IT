---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-4.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.4.4 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Unità 2.4.4

Rilasciato a febbraio 2020

* Aggiunto: supporto appropriato per 2019.3: modifiche alle API Unity corrette che hanno interrotto l&#39;oggetto scrivibile del plug-in Substance. Oggetti rielaborati per funzionare con gli aggiornamenti API 2019.3. Fisso - L’uso di materiale personalizzato fa diventare nero il materiale al termine del gioco
* Corretto - Arresto anomalo quando si utilizza la funzione Duplicate() in uno script, quindi si entra e si esce dalla riproduzione.
* Fisso - Ripristino di affiancamento, impostazioni e shader dei materiali nel 2019.3
* Fisso - HDRP Material Shader non aggiorna le modifiche apportate a un parametro
* Corretto: la mappa della maschera HDRP non viene aggiornata
* Fisso - Aggiungi parametro stringa per funzione duplicata
* Fisso - Correggi il supporto Linux nella versione più recente di Unity stabile
* Corretto: problema relativo all’indirizzo del codice bitcode che deve essere disattivato per iOS

Problemi noti:

* Se si rinomina la risorsa HDRP, il plug-in non genera una Mappa maschera.
* Quando si utilizza il plug-in Substance in un progetto HDRP, l’utilizzo della compressione Nessuna imposta le texture della scala di grigi sull’Alpha 8.
* GameObjects viene deselezionato in modalità di riproduzione
* Se fai clic su &quot;Genera mappe mappa mappa&quot; in un grafico a Substance in modalità di riproduzione, la modifica dei parametri determina un blocco infinito.
