---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: Combina più materiali Substance in fase di runtime in Unreal Engine 5 utilizzando i nodi di aggregazione Blueprint per flussi di lavoro avanzati.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance aggregata Blueprint(UE5)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Blueprint(UE5): Substance aggregata

1. Utilizzare il nodo &quot;Create Aggregate Substance Factory&quot; e impostare Output and Input Factory. La fabbrica di output deve disporre di una mappa texture da utilizzare come immagine di input nei parametri della fabbrica di input.
1. Crea oggetti SubstanceConnection per ogni texture di output utilizzata come input con i nomi dei valori corrispondenti (il nome di output dal grafico di output e il nome del parametro di input dal grafico di input)
1. Aggiungete un nodo Crea istanza grafico e inserite il risultato del nodo &quot;Crea fabbrica di Substance aggregate&quot; nell&#39;input Factory insieme a un materiale principale da usare come modello (questo può essere uno dei materiali predefiniti\_substance inclusi con il plug-in).
1. Creare una variabile di istanza di Grafico Substance e memorizzare il risultato del nodo precedente.
1. Facoltativo: impostare i parametri di sostanza desiderati (questo esempio imposta una nuova risoluzione per gli output del grafico).
1. Create un nodo di rendering asincrono o sincrono e collegate le istanze da sottoporre a rendering alla variabile di istanza di Grafico Substance.
1. Utilizzate la funzione &quot;Ottieni istanza di materiale dinamica&quot; dall&#39;istanza del grafico per creare o ottenere un&#39;istanza di materiale esistente. Se lasciate vuoto il campo Nome (Name) e Nel materiale principale (In Parent Material), vengono utilizzati i parametri utilizzati per generare l&#39;istanza al punto 3.
1. Aggiungete un Set Material Node e impostate il valore della variabile MID come Material Input. Per la destinazione, impostatela sull’oggetto a cui desiderate applicare il materiale.
