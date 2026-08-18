---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/what-is-baking.html"
breadcrumb-title: ''
description: Scoprite cos'è il baking e scoprite come salvare le informazioni sulla trama 3D nei file di texture per migliorare i materiali Substance.
helpx_creative_field: ""
helpx_description: "bakers > Getting Started > What is Baking "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Che cos’è Baking '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---


# Che cos&#39;è Baking?

![](https://upload.wikimedia.org/wikipedia/commons/3/36/Normal_map_example.png)

&#x200B;>> 

(crediti: [Paolo Cignoni](https://commons.wikimedia.org/wiki/File:Normal_map_example.png) - [CC BY-SA 1.0](https://creativecommons.org/licenses/by-sa/1.0)

Baking è il nome del processo relativo al **salvataggio delle informazioni** relative a una **trama 3D** in un file **texture** ([bitmap](https://en.wikipedia.org/wiki/Raster_graphics)). Nella maggior parte dei casi questo processo coinvolge un’altra trama. In questo caso, le informazioni della prima trama vengono trasferite sugli UV della seconda trama e quindi salvate in una texture.

Mentre alcune applicazioni possono supportare le informazioni di cottura nelle proprietà della trama (come i colori dei vertici), Substance Bakers consente di infornare le informazioni solo fino a una texture. Tuttavia, possono leggere le proprietà della trama e applicarle alle texture (come i colori dei vertici).

## È necessario cuocere?

Il software Substance genera texture che possono essere migliorate utilizzando informazioni relative alla geometria della trama.\
Molti filtri e materiali possono adattarsi alla geometria specifica di una trama 3D osservando le texture cotte. Baking può fornire informazioni su dove possono trovarsi le ombre ambientali, dove sono i bordi della geometria e molto altro.

Ad esempio: una vecchia auto potrebbe avere una ruggine applicata nella parte inferiore perché non si è mossa per un po&#39;. La cottura della mappa di posizione consentirà di sapere dove si trova il fondo sulla trama che alimenterà il generatore di ruggini e produrrà la texture adattata.

![](../../assets/examples.jpg){width="500px"}

## Come funziona la cottura al forno?

Ogni panettiera esegue azioni specifiche per generare il proprio risultato, ma in generale il processo di cottura prevede due metodi possibili:

* **Baking su una trama**: utilizza la trama corrente per generare informazioni.
* **Baking da una trama a un&#39;altra**: calcola le informazioni da una trama di origine e trasferisce il risultato in un&#39;altra trama.

Questo processo di cottura si basa sulle proprietà della trama, motivo per cui la trama deve essere pulita ed esente da possibili difetti nella sua geometria.

## Che tipo di informazioni puoi fare?

Molti tipi di informazioni possono essere analizzati. Tuttavia, in generale, è necessario solo un insieme specifico, in quanto può essere estrapolato per creare risultati più avanzati in un secondo momento. Questo è il motivo per cui ci sono un tipo comune di processo di cottura che può essere trovato in più software.

Ad esempio, un software di Substance è in grado di generare il seguente tipo di informazioni:

* **occlusione ambiente** (ombre ambiente)
* Informazioni **Normale** (variazioni dei dettagli della superficie memorizzate come direzioni vettoriali)
* **Direzione** (in alto o in basso, a sinistra o a destra e così via)
* **Curvatura** (bordi e cavità della geometria)
* **Posizione** (posizione relativa della geometria in un cubo normalizzato)

Per ulteriori informazioni, consultare la [documentazione di ciascun fornaio](../../bakers-settings/bakers-settings.md).

## Differenza tra forni &quot;regolari&quot; e &quot;da trama&quot;

A seconda del processo, i baker utilizzano varie implementazioni. In generale, i produttori di **da trama** si basano su tecniche di ray tracing per estrarre e proiettare i dati da un modello all&#39;altro.
