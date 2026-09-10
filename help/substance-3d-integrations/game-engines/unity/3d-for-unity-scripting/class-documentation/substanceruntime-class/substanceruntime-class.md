---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntime-class.html"
breadcrumb-title: ''
description: Documentazione di riferimento per la classe SubstanceRuntime utilizzata per le operazioni sui materiali di Substance in fase di runtime in Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntime Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Classe SubstanceRuntime
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 1%

---


# Classe SubstanceRuntime

## Riferimento alla classe Adobe.Substance.Runtime.SubstanceRuntime

Classe Singleton che gestisce l&#39;inizializzazione del motore di Substance e viene utilizzata per ottenere i gestori nativi delle istanze di substance.\
Diagramma di ereditarietà per Adobe.Substance.Runtime.SubstanceRuntime:

![](../../../../../assets/image2022-6-22-14-35-28.png)

### Funzioni membro pubblico

```
• SubstanceNativeGraph InitializeInstance (SubstanceGraphSO substanceInstance)
```


Crea un handle SDK di Substance per un determinato SubstanceGraphSO.

### Proprietà

```
• static SubstanceRuntime Instance [get]
```


Singleton.

### Descrizione dettagliata

Classe Singleton che gestisce l&#39;inizializzazione del motore di Substance e viene utilizzata per ottenere i gestori nativi delle istanze di substance.

### Documentazione sulle funzioni membro

#### InitializeInstance()

```
SubstanceNativeGraph Adobe.Substance.Runtime.SubstanceRuntime.InitializeInstance  

( SubstanceGraphSO substanceInstance ) [inline]
```


Crea un handle SDK di Substance per un determinato SubstanceGraphSO.

**Parametri**

|  |  |
| --- | --- |
| substanceInstance | SubstanceGraphSO di destinazione |


**Restituzioni**

Handle che comunica con Substance SDK

### Documentazione delle proprietà

#### Istanza

```
SubstanceRuntime Adobe.Substance.Runtime.SubstanceRuntime.Instance [static], [get]
```


Singleton.

Singleton globale.

>[!NOTE]
>
> NativeGraph.InRenderWork è destinato solo all&#39;uso interno per comunicare con la Substance Engine e non deve essere utilizzato per flussi di lavoro personalizzati.
