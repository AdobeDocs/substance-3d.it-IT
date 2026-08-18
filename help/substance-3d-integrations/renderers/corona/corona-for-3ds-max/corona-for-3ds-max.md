---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona/corona-for-3ds-max.html"
breadcrumb-title: ''
description: Usa i materiali Substance con il modulo di rendering Corona in 3ds Max utilizzando il flusso di lavoro Specular/lucidità e le mappe richieste.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona > Corona for 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corona per 3ds Max
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Corona per 3ds Max

## Substance nel plug-in Maya

![](../../../assets/scene-001v03.jpg)

## Corona 1,6 - 6

Utilizzando il plug-in [3ds Max](../../../3d-applications/3ds-max/3ds-max.md), puoi scegliere Corona nel menu Substance per impostare automaticamente il materiale Corona con gli input della texture Substance.

![](../../../assets/corona.png){width="500px"}

## Corona 7 - 9

Per il rendering Corona 7 e versioni successive, la selezione di &quot;Substance a Corona&quot; con il nodo Substance 2 selezionato creerà una rete per il materiale fisico Corona.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/corona-physical-material?$png$&jpegSize=200&wid=857)

* **LiftGamaGain** viene creato tra l’output del colore di base e l’input del colore di base. Per correggere la differenza di colore si utilizza un valore gamma di 0,455.
* **CoronaNormal** viene creato tra l&#39;output Normal e l&#39;input Base bump, nonché tra l&#39;output Coat Normal e l&#39;input Clearcoat Bump. Le impostazioni non vengono modificate, ma qui è possibile apportare modifiche per la modalità normale.
* **CoronaMix** viene creato tra l&#39;output del Colore di lucentezza e l&#39;input del Colore di lucentezza. Viene impostato un valore di Quantità mix pari a 0 e un moltiplicatore pari a 2 per il Livello base. Gli utenti possono regolare il valore Quantità mix per controllare la brillantezza.
