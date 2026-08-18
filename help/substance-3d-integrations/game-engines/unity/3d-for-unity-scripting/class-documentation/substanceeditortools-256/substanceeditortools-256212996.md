---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceeditortools-256212996.html"
breadcrumb-title: ''
description: Documentazione di riferimento per la classe SubstanceEditorTools utilizzata per la gestione del materiale Substance in Unity.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceEditorTools
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# SubstanceEditorTools

## Riferimento alla classe Adobe.SubstanceEditor.SubstanceEditorTools

Strumenti e utilità che gli utenti possono utilizzare negli script dell&#39;editor.

Diagramma di ereditarietà per Adobe.SubstanceEditor.SubstanceEditorTools:

![](../../../../../assets/image2022-10-14-17-53-23.png)

### Funzioni pubbliche statiche dei membri

```
• static void SetGraphFloatInput (SubstanceGraphSO graph, int inputId, float value)
```


Imposta l&#39;input float del grafico.

```
• static void SetGraphFloat2Input (SubstanceGraphSO graph, int inputId, Vector2 value)
```


Imposta l&#39;input del grafico float2.

```
• static void SetGraphFloat3Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


Imposta l&#39;input del grafico float3.

```
• static void SetGraphFloat4Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


Imposta l&#39;input del grafico float4.

```
• static void SetGraphIntInput (SubstanceGraphSO graph, int inputId, int value)
```


Imposta il grafico come input.

```
• static void SetGraphInt2Input (SubstanceGraphSO graph, int inputId, Vector2Int value)
```


Imposta l&#39;input del grafico int2.

```
• static void SetGraphInt3Input (SubstanceGraphSO graph, int inputId, Vector3Int value)
```


Imposta l&#39;input int3 del grafico.

```
• static void SetGraphInt4Input (SubstanceGraphSO graph, int inputId, int value0, int value1, int value2, int value3)
```


Imposta l&#39;input del grafico int4.

```
• static void SetGraphInputString (SubstanceGraphSO graph, int inputId, string value)
```


Imposta l&#39;input della stringa del grafico.

```
• static void SetGraphInputTexture (SubstanceGraphSO graph, int inputId, Texture2D value)
```


Impostate l&#39;input della texture del grafico.

```
• static void RenderGraph (SubstanceGraphSO graph)
```


Esegue il rendering del grafico di destinazione e aggiorna le relative risorse.

```
• static string CreatePresetFromCurrentState (SubstanceGraphSO graph)
```


Crea un file XML predefinito dallo stato corrente dell’oggetto grafico.

```
• static List< SubstanceGraphSO > GetGraphs (this SubstanceFileSO fileSO)
```


Restituisce l&#39;elenco degli oggetti SubstanceGraphSO associati a un oggetto SubstanceFileSO.
