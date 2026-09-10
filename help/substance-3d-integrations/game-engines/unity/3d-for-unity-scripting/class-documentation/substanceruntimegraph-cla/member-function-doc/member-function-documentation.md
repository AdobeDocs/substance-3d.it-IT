---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class/member-function-documentation.html"
breadcrumb-title: ''
description: Documentazione dettagliata per tutte le funzioni membro della classe SubstanceRuntimeGraph nello scripting Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class > Member Function Documentation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Documentazione sulle funzioni membro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%

---


# Documentazione sulle funzioni membro

## AttachGraph()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.AttachGraph  

( SubstanceGraphSO graph ) [inline]
```


Associa un nuovo oggetto grafico a questo gestore di runtime.

**Parametri**

|  |  |
| --- | --- |
| grafico | Grafico della sostanza di destinazione. |

### CreatePresetFromCurrentState()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.CreatePresetFromCurrentState ( ) [inline]
```


Salva lo stato corrente del grafico in un file XML predefinito.

**Restituzioni**

Predefinito creato utilizzando lo stato corrente degli input del grafico.

### GetGeneratedTextures()

```
List< Texture2D > Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetGeneratedTextures ( ) [inline]
```


Restituisce un elenco con tutte le texture di output per l&#39;istanza substance.

**Restituzioni**

Texture di output.

### GetInputBool()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputBool ( string inputName ) [inline]
```


Ottieni input booleano Substance.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR. |


**Restituzioni**

Valore di input corrente.

### GetInputColor()

```
Color Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputColor ( string inputName ) [inline]
```


Ottieni colore Substance

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputDescription()

```
SubstanceInputDescription Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputDescription ( string inputName ) [inline]
```


Restituisce la descrizione di input completa per il nome di input di destinazione.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome di input di destinazione. |


**Restituzioni**

Descrizione di input completa per l&#39;input di destinazione.

### GetInputFloat()

```
float Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputFloat ( string inputName ) [inline]
```


Ottieni input Virgola mobile Substance

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputInt()

```
int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputInt ( string inputName ) [inline]
```


Ottieni input Substance

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputString()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputString ( string inputName ) [inline]
```


Ottieni input stringa Substance.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Immettere il valore corrente.

### GetInputVector2()

```
Vector2 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2 ( string inputName ) [inline]
```


Ottieni input Substance vettoriale2

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputVector2Int()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2Int ( string inputName ) [inline]
```


Ottieni matrice di 2 int.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputVector3()

```
Vector3 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3 ( string inputName ) [inline]
```


Ottieni input Substance Vector3.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputVector3Int()

```
Vector3Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3Int ( string inputName ) [inline]
```


Ottieni una matrice di 3 int (valori x, y e z di Vector3Int)

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputVector4()

```
Vector4 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4 ( string inputName ) [inline]
```


Ottieni input Substance vettoriale4

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetInputVector4Int()

```
int[] Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4Int ( string inputName ) [inline]
```


Ottieni una matrice di 4 int (valori x, y, z e w di Vector4Int)

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |


**Restituzioni**

Valore di input corrente.

### GetOutputTexture()

```
Texture2D Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetOutputTexture ( string outputName ) [inline]
```


Restituisce la texture di output per un nome di output specificato.

**Parametri**

|  |  |
| --- | --- |
| outputName | Nome output. |


**Restituzioni**

Texture di output.

### GetTexturesResolution()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetTexturesResolution ( ) [inline]
```


Restituisce la risoluzione dell&#39;output della texture di istanza.

**Restituzioni**

Risoluzione di output corrente.

### HasInput()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.HasInput ( string inputName ) [inline]
```


Restituisce true se l&#39;istanza di substance ha un input con un nome specificato.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome di input. |


**Restituzioni**

TRUE se l&#39;istanza di substance ha un input con il nome specificato.

### LoadPreset()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.LoadPreset ( string presetXML ) [inline]
```


Utilizza un codice XML predefinito per impostare i parametri di input del grafico.

**Parametri**

|  |  |
| --- | --- |
| presetXML | Dati XML predefiniti. |

### RenderAsync()

```
Task Adobe.Substance.Runtime.SubstanceRuntimeGraph.RenderAsync ( ) [inline]
```


Esegue il rendering asincrono dell&#39;istanza di substance.

**Restituzioni**

Attività che verrà completata al termine del rendering.

### SetInputBool()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputBool ( string inputName, 

bool value ) [inline]
```


Aggiorna input booleano Substance

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputColor()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputColor ( string inputName, 

Color value ) [inline]
```


Aggiorna input colore Substance

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputFloat()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputFloat ( string inputName, 

float value ) [inline]
```


Aggiorna input Substance float

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputInt()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputInt ( string inputName, 

int value ) [inline]
```


Aggiorna input int Substance

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputString()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputString ( string inputName, 

string value ) [inline]
```


Aggiorna input stringa Substance.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputTexture()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputTexture (string inputName, 

Texture2D value ) [inline]
```


Aggiorna input Substance Texture2D.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputVector2()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2 ( string inputName, 

Vector2 value ) [inline]
```


Aggiorna input Substance vettoriale2

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputVector2Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2Int ( string inputName, 

Vector2Int value ) [inline]
```


Aggiorna input Substance Vector2Int.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputVector3()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3 ( string inputName, 

Vector3 value ) [inline]
```


Aggiorna input Substance Vector3

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputVector3Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3Int ( string inputName, 

Vector3Int value ) [inline]
```


Aggiorna input Substance Vector3Int.

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputVector4()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4 ( string inputName, 

Vector4 value ) [inline]
```


Aggiorna input Substance vettoriale4

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| valore | Valore utilizzato per aggiornare il parametro |

### SetInputVector4Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4Int ( string inputName, 

int x, 

int y, 

int z, 

int w ) [inline]
```


Aggiorna input Substance Vector4Int

**Parametri**

|  |  |
| --- | --- |
| inputName | Nome dell&#39;input nella SBSAR |
| x | Valore utilizzato per aggiornare il parametro |
| y | Valore utilizzato per aggiornare il parametro |
| z | Valore utilizzato per aggiornare il parametro |
| w | Valore utilizzato per aggiornare il parametro |

### SetTexturesResolution()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetTexturesResolution ( Vector2Int size ) [inline]
```


Imposta la risoluzione di output della texture di istanza.

**Parametri**

|  |  |
| --- | --- |
| dimensione |  |
