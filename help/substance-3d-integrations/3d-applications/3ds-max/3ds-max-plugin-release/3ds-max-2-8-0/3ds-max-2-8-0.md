---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-8-0.html"
breadcrumb-title: ''
description: Consultate le note sulla versione per il plug-in 3ds Max versione 2.8.0 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 3ds Max 2.8.0

<b>Aggiunto/Aggiornato:
</b>

* Supporto per la visibilità condizionale dei parametri (&#39;visible if&#39;); i parametri verranno nascosti quando le condizioni non vengono soddisfatte, mentre i rispettivi gruppi rimarranno visibili.
* Il modulo di rendering Corona è stato aggiornato alla versione 10 nel plug-in 3ds Max, migliorando le funzionalità di rendering e
* L’aggiornamento più recente migliora notevolmente la velocità di rendering e l’utilizzo della CPU in 3ds Max 2024 quando si utilizza Substance, allineando le prestazioni più strettamente con l’efficienza osservata in 3ds Max 2022.

<b>Corretto:</b>

* È stato migliorato il plug-in Substance per limitare i valori di input della tastiera all&#39;interno dell&#39;intervallo pratico per ciascun parametro, evitando problemi con il controllo del cursore e la regolazione manuale dei valori.
* È stato risolto un problema a causa del quale la copia delle conversioni delle texture Substance2 (.sbsar) nell&#39;editor materiale di slate causava un&#39;istanza involontaria del nodo copiato, causando potenzialmente arresti anomali relativi a d3d11.dll.
* È stato risolto un problema di arresto anomalo in 3ds Max durante il rendering di sostanze copiate personalizzate/modificate (.sbsar) con Corona Interactive.
* È stato risolto un problema nel nodo Substance2 di 3ds Max a causa del quale i cursori per i valori Integer 3 e 4 non rispondevano e solo la voce numerica manuale aggiornava i valori. Inoltre, questi valori non venivano visualizzati correttamente nel formato a virgola mobile. I cursori ora sono funzionali e riflettono accuratamente i tipi di valore desiderati.
* È stato risolto un problema in 3ds Max 2021 con Rendering Corona in cui i materiali delle Substance venivano visualizzati correttamente nella finestra della vista, ma renderizzati in grigio quando i file venivano trasferiti a un altro PC. Gli utenti non devono più impostare i materiali da zero o caricare i predefiniti per il rendering corretto.
* È stato risolto un problema di arresto anomalo nel plug-in 3ds Max durante il tentativo di duplicare i nodi Substance nell&#39;editor materiale di Slate.
* È stato risolto un problema a causa del quale l’impostazione Limite core CPU nel plug-in Substance non veniva salvata dopo il riavvio di 3ds Max, affinché i valori configurati dall’utente ora persistessero nelle sessioni.

Questa versione è disponibile per 3ds Max 2021, 2022 e 2023
