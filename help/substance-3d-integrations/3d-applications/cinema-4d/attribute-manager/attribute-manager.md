---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/cinema-4d/attribute-manager.html"
breadcrumb-title: ''
description: Usate Gestione attributi di Cinema 4D per configurare le proprietà delle risorse Substance e le impostazioni dei materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Attribute Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestione attributi
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Gestione attributi

Esiste una nuova modalità per le risorse Substance in Gestione attributi di Cinema 4D.

Quando si seleziona una Substance in Gestione risorse Substance, Gestione attributi passa automaticamente alla modalità Substance risorse. È inoltre possibile passare manualmente a questa modalità nel menu della modalità di Gestione attributi.

In modalità risorsa Substance puoi accedere a tutti gli ingressi di una Substance e puoi anche avere una panoramica di tutti i canali di output.

![](../../../assets/cinema-4d-9.png){width="500px"}

## Raggruppamento degli input della Substance

Se gli input di una Substance sono raggruppati, questi gruppi vengono visualizzati come tali in Gestione attributi. Sono presenti due gruppi predefiniti: **Proprietà di base** e **Input immagine**.

* Nel gruppo Proprietà di base vengono visualizzati tutti gli input non assegnati a un Substance Designer nel gruppo.
* Come già indicato nel nome, tutti gli input della Substance che si collegano a immagini esterne vengono raccolti nel gruppo Input immagine.

## Parametro Filename

Utilizzando il parametro Filename in Gestione attributi, la posizione del file delle risorse Substance può essere modificata dopo che sono state caricate in una scena.

![](../../../assets/cinema-4d-10.png){width="500px"}

Ciò può essere utile non solo per spostare i file di Substance, ma anche quando si scambia una Substance con una completamente diversa.

In questo caso, all’utente verrà chiesto se eventuali riferimenti esistenti a canali di output della Substance precedenti devono essere rimappati alla nuova Substance.

![](../../../assets/cinema-4d-11.png){width="500px"}

Se alla domanda viene risposto &#39;No&#39;, i collegamenti alla Substance precedente verranno eliminati da tutti gli shader di Substance. Per rimappare i canali di output, il plug-in cercherà prima i canali di output con lo stesso tipo e poi con lo stesso nome.

## Tristato parametro

Se si selezionano più Substance contemporaneamente, gli ingressi condivisi tra queste Substance vengono visualizzati come tristato e possono essere modificati contemporaneamente per tutte le Substance selezionate (come tutti gli altri parametri nelle Cinema 4D).

In questi casi, i canali di output verranno visualizzati come mostrato di seguito.

![](../../../assets/cinema-4d-12.png){width="300px"}
