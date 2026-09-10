---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/api-overview.html"
breadcrumb-title: ''
description: Panoramica di riferimento dell’API Substance Unity obsoleta per progetti legacy e esigenze di scripting.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > API Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panoramica delle API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# Panoramica delle API

## Substance.Game

```
Using Substance.Game
```


Substance.Game è l&#39;assembly che contiene le classi utilizzate per la creazione di script. Tali classi sono le seguenti:

**Substance.Gioco.**&#x200B;**Substance**: fa riferimento alla sbsar

**Substance.Game.SubstanceGraph**: grafico individuale nella sbsar.*(utilizzato come materiale procedurale in Unity 2017)*

## Processo di scripting

1. Creare un&#39;istanza di SubstanceGraph
1. Impostate i parametri sull&#39;istanza del grafico.
1. Inserisci in coda la Substance per il rendering: QueueForRender() aggiungerà il grafico Substance a una coda. Questo elenco verrà elaborato dalla prossima chiamata a RenderAsync o RenderSync.

### Parametri dell’istanza del grafico

```
// panel color 

mySubstance.SetInputColor("paint_color", color); 

 

// panel size 

mySubstance.SetInputVector2("square_open", panelSize); 

 

// wear level 

mySubstance.SetInputFloat("wear_level", wearLevel);
```


Il valore tra virgolette è l&#39;Identificatore di parametro impostato in Substance Designer.

In Ispettore unità, puoi passare il mouse su un parametro per visualizzare una descrizione che mostra il nome dell&#39;Identificatore impostato nel Substance Designer.

![](../../../../assets/tooltip-6.png)

### Inserisci in coda la sostanza per il rendering

```
// queue the substance to render 

mySubstance.QueueForRender(); 

 

//render all substances async 

Substance.Game.Substance.RenderAsync();
```


![](../../../../assets/unityscript.gif)

>[!NOTE]
>
> Al momento, supportiamo solo l&#39;architettura x86\_64. È necessario impostare x86\_64 nelle Impostazioni di compilazione

![](../../../../assets/arch.png)
