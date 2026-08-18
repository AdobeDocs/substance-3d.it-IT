---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: Comprendere in che modo la triangolazione della trama influisce sui risultati di cottura e apprendere le procedure ottimali per la preparazione della geometria.
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Triangolazione prima della cottura
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Triangolazione prima della cottura

Le trame 3D possono essere definite con poligoni con più bordi per faccia. Di solito tramite quad (4 spigoli), a volte di più (n-goni).\
Il software tuttavia trasforma questi poligoni in triangoli in un secondo momento, perché è più facile gestire ed eseguire il calcolo con (in particolare sulla GPU).

## In che modo la triangolazione può influire su una trama?

![](../../assets/triangulation.jpg)

**nessuna soluzione standard** per convertire Quad/N-Gons in triangoli. Come illustrato nell&#39;immagine precedente, sono valide più scelte.\
È improbabile che i panettieri triangolino trame come farebbe un motore di gioco perché scegliamo un algoritmo specifico su un altro.

## Perché triangolare prima di cuocere?

Il processo di cottura legge la geometria e quindi codifica le informazioni in texture.\
Poiché tali informazioni sono basate sugli UV e talvolta sulla topologia della trama, altri software potrebbero decodificare le informazioni in modo errato se non leggono la geometria allo stesso modo di quando applicano la texture.

Nell’immagine seguente, potete vedere la trama low-poly in alto a sinistra e quella high-poly in alto a destra.\
In basso c&#39;è il polo basso con la mappa normale ricavata dal polo alto. La trama a sinistra usa una triangolazione identica a quella usata dalla Substance Painter durante la cottura. La trama a destra non visualizza e mostra artefatti neri. Questo perché non c&#39;è corrispondenza tra il modo in cui la mappa normale è stata cotta e il modo in cui la trama è attualmente triangolata. Questo problema può essere risolto **aggiornando la trama e/o riattivando**.

![](../../assets/example-triangulation-artifact.jpg)
