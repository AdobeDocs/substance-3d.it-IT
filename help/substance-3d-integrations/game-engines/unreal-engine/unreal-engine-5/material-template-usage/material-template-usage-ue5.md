---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5.html"
breadcrumb-title: ''
description: Creazione e utilizzo di modelli di materiale in Unreal Engine 5 per definire il modo in cui i nodi di output Substance si connettono agli input di materiale.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Uso modello materiale - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# Uso modello materiale - UE5

I Modelli di materiale consentono all&#39;utente di creare un materiale di base per le sostanze da utilizzare come modello per collegare i loro nodi di output agli input nel materiale.\
Verranno automaticamente utilizzati gli output con lo stesso nome e tipo di un input di materiale. Questo esempio di materiale principale ha un nodo di esempio di texture &quot;baseColor&quot; che verrà riempito se la Substance ha un output di texture denominato anche &quot;baseColor&quot;.\
![](../../../../assets/parent-material-sample.png)

Gli output Substance supportano l’aggiornamento di texture, valori a virgola mobile singola o scalare int e valori vettoriali (2-4). Per utilizzare output float o int in fase di runtime, è necessario ottenere l&#39;elemento dynamicMaterialInstance dal grafico, poiché constantMaterialInstances (qualsiasi materiale generato nell&#39;editor) non può modificare i valori scalari in fase di runtime.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/scalar-value?$png$&jpegSize=100&wid=245)

L’istanza del grafico della sostanza tenterà di inserire tutti i valori di output pertinenti al momento della creazione.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-04-01-at-4-38-31-pm?$png$&jpegSize=200&wid=1076)
