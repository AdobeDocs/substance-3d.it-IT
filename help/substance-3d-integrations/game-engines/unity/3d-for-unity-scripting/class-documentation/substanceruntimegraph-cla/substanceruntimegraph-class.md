---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class.html"
breadcrumb-title: ''
description: Documentazione di riferimento per la classe SubstanceRuntimeGraph utilizzata per le operazioni dei grafici di runtime in Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Classe SubstanceRuntimeGraph
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Classe SubstanceRuntimeGraph

## Riferimento alla classe Adobe.Substance.Runtime.SubstanceRuntimeGraph

Classe che fornisce funzionalità di runtime per modificare gli input e eseguire il rendering dei grafici delle sostanze, consentendo a Substance←GraphSO di generare le proprie risorse in fase di runtime.

Diagramma di ereditarietà per Adobe.Substance.Runtime.SubstanceRuntimeGraph:

![](../../../../../assets/image2022-10-14-17-53-23-1.png)

### Funzioni membro pubblico

```
• void AttachGraph (SubstanceGraphSO graph)
```


Associa un nuovo oggetto grafico a questo gestore di runtime.

```
• void SetInputFloat (string inputName, float value)
```


Aggiorna input Virgola mobile Substance

```
• float GetInputFloat (string inputName)
```


Ottieni input Virgola mobile Substance

```
• void SetInputVector2 (string inputName, Vector2 value)
```


Aggiorna input Substance vettoriale2

```
• Vector2 GetInputVector2 (string inputName)
```


Ottieni input Substance vettoriale2

```
• void SetInputVector3 (string inputName, Vector3 value)
```


Aggiorna input Substance Vector3

```
• Vector3 GetInputVector3 (string inputName)
```


Ottieni input Substance Vector3.

```
• void SetInputVector4 (string inputName, Vector4 value)
```


Aggiorna input Substance vettoriale4

```
• Vector4 GetInputVector4 (string inputName)
```


Ottieni input Substance vettoriale4

```
• void SetInputColor (string inputName, Color value)
```


Aggiorna input colore Substance

```
• Color GetInputColor (string inputName)
```


Ottieni colore Substance

```
• void SetInputBool (string inputName, bool value)
```


Aggiorna input booleano Substance

```
• bool GetInputBool (string inputName)
```


Ottieni input booleano Substance.

```
• void SetInputInt (string inputName, int value)
```


Aggiorna input int Substance

```
• int GetInputInt (string inputName)
```


Ottieni input Substance

```
• void SetInputVector2Int (string inputName, Vector2Int value)
```


Aggiorna input Substance Vector2Int.

```
• Vector2Int GetInputVector2Int (string inputName)
```


Ottieni matrice di 2 int.

```
• void SetInputVector3Int (string inputName, Vector3Int value)
```


Aggiorna input Substance Vector3Int.

```
• Vector3Int GetInputVector3Int (string inputName)
```


Ottieni una matrice di 3 int (valori x, y e z di Vector3Int)

```
• void SetInputVector4Int (string inputName, int x, int y, int z, int w)
```


Aggiorna input Substance Vector4Int

```
• int[ ] GetInputVector4Int (string inputName)
```


Ottieni una matrice di 4 int (valori x, y, z e w di Vector4Int)

```
• void SetInputString (string inputName, string value)
```


Aggiorna input stringa Substance.

```
• string GetInputString (string inputName)
```


Ottieni input stringa Substance.

```
• SubstanceInputDescription GetInputDescription (string inputName)
```


Restituisce la descrizione di input completa per il nome di input di destinazione.

```
• void SetInputTexture (string inputName, Texture2D value)
```


Aggiorna input Substance Texture2D.

```
• Vector2Int GetTexturesResolution ()
```


Restituisce la risoluzione di output della texture di istanza.

```
• void SetTexturesResolution (Vector2Int size)
```


Imposta la risoluzione di output della texture di istanza.

```
• bool HasInput (string inputName)
```


Restituisce true se l&#39;istanza di substance ha un input con un nome specificato.

```
• List< Texture2D > GetGeneratedTextures ()
```


Restituisce un elenco con tutte le texture di output per l&#39;istanza substance.

```
•  Texture2D GetOutputTexture (string outputName)
```


Restituisce la texture di output per un nome di output specificato.

```
• void Render ()
```


Esegue il rendering dell&#39;istanza substance in modo sincrono.

```
• Task RenderAsync ()
```


Esegue il rendering asincrono dell&#39;istanza di substance.

```
• void LoadPreset (string presetXML)
```


Utilizza un codice XML predefinito per impostare i parametri di input del grafico.

```
• string CreatePresetFromCurrentState ()
```


Salva lo stato corrente del grafico in un file XML predefinito.

## Attributi pubblici

```
• SubstanceGraphSO GraphSO
```


Istanza della sostanza di destinazione.

## Funzioni membro protette

```
• void Awake ()
```


SubstanceRuntime sveglio verrà utilizzato per creare un&#39;istanza per SubstanceGraphSO allegato nella sostanza

SDK

```
• void Update ()
```


Controlla i risultati del rendering nella Coda concorrente di rendering.

```
• void OnDestroy ()
```


Dispone il gestore SDK substance.

## Proprietà

```
• Material DefaulMaterial [get]
```


Materiale principale generato dall&#39;istanza di substance.
