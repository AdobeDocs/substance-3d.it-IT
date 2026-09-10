---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-substance-material-parameters.html"
breadcrumb-title: ''
description: Modificate i parametri del materiale Substance in fase di runtime in Unreal Engine 4 utilizzando i nodi di Blueprint per il controllo dinamico del materiale.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Substance material parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parametri del materiale della Substance Blueprint(UE4)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# Blueprint(UE4): Substance parametri materiale

## Modifica di un parametro float:

Per modificare i parametri float, color(float4) e booleano della sostanza, utilizzare il [nodo Float di input](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/integrations/blueprint-node-reference-151584784.html).

1. Create una variabile con un tipo di &quot;Istanza di Grafico Substance&quot; come riferimento.
1. Creare un set di nodi mobili di input e impostare la destinazione come variabile dell&#39;istanza di Grafico Substance.
1. Nel nodo Set Input Float, impostare Identifier come nome del parametro Substance da modificare.\
   *\* È possibile trovare il nome dell&#39;identificatore aprendo la Substance INST e passando il mouse sul nome del parametro. Il nome dell&#39;identificatore verrà visualizzato nel popup della descrizione comandi.*
1. Nel nodo mobile di input, trascinare una connessione e creare un nodo Crea array. Il nodo Crea matrice avrà un indice pari a 0. L’indice 0 corrisponde al valore float.
1. Crea un nodo di rendering asincrono o sincrono e collega la linea di esecuzione dall’opzione Imposta dispositivo di input al nodo di rendering. Impostate le istanze da sottoporre a rendering sulla variabile di istanza di Grafico Substance.\
   *\* Async non blocca e Sync blocca.*

![](../../../../../assets/steps.png){width="800px"}

## Parametri booleani

I parametri booleani vengono modificati utilizzando Set Input Bool.

![](../../../../../assets/setbool.png){width="800px"}

## Parametri colore

I parametri del colore vengono modificati utilizzando Imposta colore di input.

![](../../../../../assets/setcolor.png){width="800px"}

## Modifica di un parametro Integer:

I parametri di tipo Integer funzionano allo stesso modo del parametro Set Input Float. Verrà utilizzato il nodo Intero di input impostato.

![](../../../../../assets/int.png)

## Identificatori

Potete trovare l&#39;identificatore di un parametro in SUBSTANCE INST. Spostate il mouse sul parametro e la descrizione comandi mostrerà il nome identificatore. Questo è il nome impostato nel campo identificatore dell&#39;output in Substance Designer.

![](../../../../../assets/indent-1.png){width="800px"}
