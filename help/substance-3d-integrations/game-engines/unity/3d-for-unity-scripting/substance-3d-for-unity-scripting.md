---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting.html"
breadcrumb-title: ''
description: Utilizza l’API di Substance 3D in Unity per scrivere script che aggiornino e modifichino i parametri Substance in fase di runtime.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Scripting per Substance 3D for Unity
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Scripting per Substance 3D for Unity

Questa sezione della documentazione contiene dettagli sulle API Substance 3D fornite tramite il plug-in Substance 3D per Unity. Utilizzando le API Substance, puoi scrivere script per aggiornare e modificare i parametri Substance in fase di runtime.

## Panoramica delle API

Il plug-in è diviso in 3 assembly diversi.

* Adobe.Substance
* Adobe.Substance.Editor
* Adobe.Substance.Runtime

### Adobe.Substance

Contiene componenti condivisi per interagire con Substance SDK e generare oggetti Unity corrispondenti. Include inoltre strutture di dati di marshalling per la comunicazione tra C# e l&#39;API C++ di Substance SDK.

#### Adobe.Substance.Editor

Contiene classi specifiche dell&#39;editor per la gestione della visualizzazione delle informazioni sugli oggetti Substance Unity e per la gestione della pipeline di importazione quando vengono aggiunti file sbsar al progetto. La classe SubstanceEditorEngine è un singleton che gestisce la durata del motore substance e di tutte le relative istanze gestite.

#### Adobe.Substance.Runtime

Questa classe include componenti che gestiranno la creazione e la gestione degli oggetti Substance durante l&#39;esecuzione in fase di esecuzione. SubstanceRuntime è l&#39;equivalente della classe SubstanceEditorEngine per il runtime. Gestirà l&#39;inizializzazione del motore substance e la creazione di istanze di qualsiasi istanza substance con cui gli script utente interagiranno.

## Utilizzo runtime

Affinché gli input dell’istanza di Substance possano essere modificati in fase di runtime, è necessario aggiungere un materiale SubstanceRuntime←- alla scena (preferibilmente allo stesso GameObject del materiale Substance). Questa classe funge da helper per l&#39;impostazione del materiale utilizzando il singleton Adobe.Substance.Runtime.SubstanceRuntime che gestisce la creazione di istanze degli oggetti SDK di Substance in fase di runtime.

## Esempi di codice

Nell&#39;esempio seguente viene illustrato come modificare i parametri di input in fase di esecuzione utilizzando SubstanceRuntimeGraph.

### Modifica dei parametri

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    // panel color 

    mySubstance.SetInputColor("paint_color", new Color(0.237 f, 0.834 f, 0.045 f, 1.0 f)); 

    // panel size 

    mySubstance.SetInputVector2("square_open", new Vector2(0.101 f, 0.209 f)); 

    // wear level 

    mySubstance.SetInputFloat("wear_level", 0.977 f); 

    // Submit async render. 

    mySubstance.RenderAsync(); 

  } 

}
```


Puoi anche utilizzare SubstanceRuntimeGraph per accedere alle informazioni di input e output sul Materiale Substance.

#### Ottieni informazioni di input

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```


Nell&#39;esempio seguente viene illustrato come creare un menu predefinito personalizzato nell&#39;editor con SubstanceEditorTools.

##### Creazione di controlli predefiniti.

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```
