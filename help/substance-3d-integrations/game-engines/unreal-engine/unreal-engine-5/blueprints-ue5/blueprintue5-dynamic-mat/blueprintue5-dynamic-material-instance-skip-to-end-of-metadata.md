---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-dynamic-material-instance-skip-to-end-of-metadata.html"
breadcrumb-title: ''
description: Create istanze dinamiche di materiale da materiali di Substance in fase di runtime in Unreal Engine 5 utilizzando Blueprint.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Dynamic Material Instance Skip to end of metadata
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5) Dynamic Material Instance Salta alla fine dei metadati
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Blueprint(UE5): istanza di materiale dinamico Salta alla fine dei metadati

1. Creare una variabile di tipo Substance Instance Factory e impostare il valore predefinito su Substance Factory importata.
1. Aggiungete un nodo Crea istanza grafico e inserite la factory dell&#39;istanza di Substance nell&#39;input Factory insieme a un materiale principale da usare come modello (può essere uno dei materiali predefiniti\_substance inclusi con il plug-in).
1. Creare un&#39;altra variabile per memorizzare l&#39;oggetto Istanza di Grafico Substance creato nel passaggio precedente.
1. Utilizzate la funzione &quot;Ottieni istanza di materiale dinamica&quot; dall&#39;istanza del grafico per creare o ottenere un&#39;istanza di materiale esistente. Se lasciate vuoto il campo Nome (Name) e Nel materiale principale (In Parent Material), vengono utilizzati i parametri utilizzati per generare l&#39;istanza al punto 2.
1. Create una variabile di tipo Materiale. Si tratta dell&#39;istanza dinamica del materiale (MID). Impostate il valore restituito da &quot;Get Dynamic Material Instance&quot; sulla variabile.

   ![](../../../../../assets/dynamic-material-annotated-1.png)
1. Aggiungete un Set Material Node e impostate il valore della variabile MID come Material Input. Per la destinazione, impostatela sull’oggetto a cui desiderate applicare il materiale.
1. Facoltativo: impostare i parametri di sostanza desiderati (in questo esempio viene utilizzata un&#39;istanza preesistente del grafico della sostanza e vengono copiati i valori in quello nuovo).
1. Create un nodo di rendering asincrono o sincrono e collegate le istanze da sottoporre a rendering alla variabile di istanza di Grafico Substance.
