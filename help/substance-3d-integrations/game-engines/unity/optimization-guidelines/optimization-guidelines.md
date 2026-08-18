---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/optimization-guidelines.html"
breadcrumb-title: ''
description: Segui le linee guida di ottimizzazione per bilanciare la complessità del materiale Substance con le prestazioni di rendering in Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Optimization Guidelines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Linee guida per l'ottimizzazione
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Linee guida per l&#39;ottimizzazione

Più complessi sono i materiali Substance, maggiore è la potenza di elaborazione necessaria per il rendering. I materiali Substance devono pertanto **bilanciare la complessità e la velocità di rendering**. Questo elemento è *particolarmente* importante se verrà utilizzato in applicazioni grafiche in tempo reale, ad esempio nei giochi.

Quando crei i tuoi materiali di Substance personalizzati, assicurati di controllare le seguenti linee guida di ottimizzazione.

[Linee guida per l&#39;ottimizzazione del Substance Designer](https://docs.substance3d.com/display/SDDOC/Performance+Optimization+Guidelines)

Un importante avvertimento da tenere presente sono i nodi che hanno una risoluzione assoluta di 4K o superiore.

>[!WARNING]
>
> **Prestare attenzione alla risoluzione e alle impostazioni di risoluzione relative ai genitori.**\
> Valori elevati influiscono negativamente sulle prestazioni, quindi è importante considerare come verrà utilizzato il materiale e se è possibile ridurre le dimensioni dei dati coinvolti.
>   
> Il motore della CPU a Substance è in grado di elaborare dati a 4K, ma è molto lento e può causare il blocco o l’arresto anomalo di un’integrazione.

Nell&#39;esempio seguente, la dimensione di output di un nodo [Tile Sampler](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/node-library/texture-generators/patterns/tile-sampler) è impostata su [Absolute](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/output-size) 4096. Ciò fa sì che diversi nodi a valle calcolino a 4K prima di essere ridimensionati per la risoluzione finale dell&#39;output del 2048.

![](../../../assets/absolute.png){width="1000px"}
