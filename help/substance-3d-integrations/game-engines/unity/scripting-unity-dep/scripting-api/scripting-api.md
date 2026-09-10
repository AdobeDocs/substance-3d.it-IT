---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/scripting-api.html"
breadcrumb-title: ''
description: Documentazione di riferimento per l’API di scripting Substance Unity obsoleta per il supporto di progetti precedenti.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API di scripting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---


# API di scripting

## Substance nell’API Unity - 2.2.0

## Substance parametri materiale

| Public, metodo | Descrizione | Parametro |
| --- | --- | --- |
| **float** *GetInputFloat*(**string** inputName) pubblico | Ottieni input Substance **Virgola mobile** | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| public **int** *SetInputFloat*(**string** inputName, valore **float**) | Aggiorna input Substance **Virgola mobile** | **Stringa** i *nputName* Nome dell&#39;input nella **Virgola mobile** *valore* SBSAR utilizzato per aggiornare il parametro |
| public **void** *SetInputVector2*(**string** inputName, valore **Vector2**) | Aggiorna input Substance **Vettoriale2** | **Stringa** *nomeInput* Nome dell&#39;input nell&#39;SBSAR **vettore2** *input* Valori utilizzati per aggiornare il parametro |
| **vettoriale2** *GetInputVector2*(**stringa** inputName) pubblico | Ottieni input Substance **Vettoriale2** | **Stringa** &quot;inputName&quot; Nome dell&#39;input nella SBSAR |
| public **void** *SetInputVector3*(**string** inputName, valore **Vector3**) | Aggiorna input Substance **Vettoriale3** | **Stringa** *nomeInput* Nome dell&#39;input nella **Vettore3** *valore* SBSAR Valori utilizzati per aggiornare il parametro |
| public **vettoriale3** *GetInputVector3*(**string** inputName) | Ottieni input Substance **Vettore3** | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| public **void** *SetInputVector4*(**string** inputName, valore **Vector4**) | Aggiorna input Substance **Vettoriale4** | **Stringa** *nomeInput* Nome dell&#39;input nell&#39;SBSAR **vettore4** *valore* Valori utilizzati per aggiornare il parametro |
| public **vettoriale4** *GetInputVector4*(**string** inputName) | Ottieni input Substance **Vector4** | **Stringa** nomeInputName dell&#39;input nella SBSAR |
| public **void** *SetInputColor*(**string** inputName, valore **Color**) | Aggiorna input Substance **Colore** | **String** inputName Nome dell&#39;input nel valore **Color** SBSAR utilizzato per aggiornare il parametro |
| public **color** *GetInputColor*(**string** inputName, **int** dataType) | Ottieni Substance **Colore** | **Stringa** *nomeInput* Nome dell&#39;input nella **stringa** *tipoDati* SBSAR |
| **void** *SetInputBool*(**string** inputName, **bool** value) pubblico | Aggiorna input Substance **booleano** | **Stringa** *nomeInput* Nome dell&#39;input nel valore **Bool** *value* SBSAR utilizzato per aggiornare il parametro |
| public **bool** *GetInputBool*(**string** inputName) | Ottieni input Substance **booleano** | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| **void** *SetInputInt*(**string** inputName, valore **int**) pubblico | Aggiorna input Substance **int** | **Stringa** *nomeInput* Nome dell&#39;input nel valore **int** *valore* SBSAR utilizzato per aggiornare il parametro |
| public **int** *GetInputInt*(**string** inputName) | Ottieni input Substance **int** | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| **void** *SetInputVector2Int*(**string** inputName, **int** x, **int** y) pubblico | Aggiorna input Substance **Vector2Int** | **String** *inputName* Nome dell&#39;input nel valore **Int** *x* SBSAR utilizzato per aggiornare il parametro **Int** y Valore utilizzato per aggiornare il parametro |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector2Int*( stringa inputName) | Ottieni una matrice di 2 int (valori x e y di Vector2Int) | **String** *inputName* Nome dell&#39;input nel valore **Int** *x* SBSAR utilizzato per aggiornare il parametro **Int** y Valore utilizzato per aggiornare il parametro |
| **void Substance.Game.SubstanceGraph**.*SetInputVector3Int*( stringa inputName, int x, int y, int z) | Aggiorna input Substance Vector3Int | **String** *inputName* Nome dell&#39;input nel valore **Int** *x* SBSAR utilizzato per aggiornare il parametro **Int** y Valore utilizzato per aggiornare il parametro **Int** z Valore utilizzato per aggiornare il parametro |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector3Int*( stringa inputName) | Ottieni una matrice di 3 int (valori x, y e z di Vector3Int) | **String** *inputName* Nome dell&#39;input nel valore **Int** *x* SBSAR utilizzato per aggiornare il parametro **Int** y Valore utilizzato per aggiornare il parametro **Int** z Valore utilizzato per aggiornare il parametro |
| **void Substance.Game.SubstanceGraph**.*SetInputVector4Int*( stringa inputName, int x, int y, int z, int w) | Aggiorna input Substance Vector4Int | **Stringa** *nomeInput* Nome dell&#39;input nel valore **int** *x* SBSAR utilizzato per aggiornare il parametro **int** y Valore utilizzato per aggiornare il parametro **int** z Valore utilizzato per aggiornare il parametro **int** w Valore utilizzato per aggiornare il parametro |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector4Int*( stringa inputName) | Ottieni una matrice di 4 int (valori x, y, z e w di Vector4Int) | **Stringa** *nomeInput* Nome dell&#39;input nel valore **int** *x* SBSAR utilizzato per aggiornare il parametro **int** y Valore utilizzato per aggiornare il parametro **int** z Valore utilizzato per aggiornare il parametro **int** w Valore utilizzato per aggiornare il parametro |
| **void Substance.Game.SubstanceGraph**.*SetInputString*( stringa inputName, valore stringa) | Aggiorna input stringa Substance | **String** *inputName* Nome dell&#39;input nella **String** *value* SBSAR utilizzata per aggiornare il parametro |
| **string Substance.Game.SubstanceGraph**.*GetInputString*( string inputName) | Ottieni input stringa di Substance | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| **void Substance.Game.SubstanceGraph**.*SetInputTexture*( stringa inputName, valore Texture2D) | Aggiorna input Substance Texture2D | **String** *inputName* Nome dell&#39;input nella **Texture2D** *value* SBSAR utilizzata per aggiornare il parametro |
| **Texture2D Substance.Game.SubstanceGraph**.*GetInputTexture*( string inputName) | Ottieni input Substance Texture2D | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| **Substance VectorInt.Game.SubstanceGraph**.*GetTexturesResolution*() | Ottenete la risoluzione delle texture delle Impostazioni di destinazione del grafico (x di Vector4Int = larghezza, y = height, i valori possono essere 32, 64, 128, 256, 512, 1024, 2048 e 4096) | Nessuno |
| **int Substance.Game.SubstanceGraph**.*SetTexturesResolution*( Dimensione Vector2Int) | Impostate la risoluzione delle texture delle Impostazioni di destinazione del grafico (x di Vector2Int = larghezza, y = height, i valori possono essere 32, 64, 128, 256, 512, 1024, 2048 e 4096) Restituisce 0 in caso di esito positivo, altrimenti restituisce -1. | **Vector2Int** *size* utilizzato per aggiornare il parametro&#x200B;**.** |
| **Substance elenco.Game.SubstanceGraph**.*GetGeneratedTextures*() | Restituisce tutti gli oggetti Substance Texture2D utilizzati dallo shader di materiale del grafico. | Nessuno |
| **int Substance.Game.SubstanceGraph**.*Bake*( Texture2D texture, string absolutePath) | Generate file .png per tutti gli oggetti Texture2D Substance utilizzati dallo shader di materiale del grafico. | Nessuno |
| **&#x200B;**&#x200B;Substance.Gioco.**&#x200B; SubstanceGraph**.*Duplicato*() | Duplicare un Grafico Substance | Nessuno |
| **Substance.Game.SubstanceGraph**.*Duplicato*(string newGraphName) | Duplica un Grafico Substance e assegnagli un nome (anche il materiale corrispondente avrà lo stesso nome) | **String newGraphName** |
| **&#x200B;**&#x200B;Substance.Game.**&#x200B; SubstanceGraph**.*GetInputProperties*() | Query informazioni di input procedurali, restituisce una matrice di &#39;InputProperties&#39;, con :public struct InputProperties { public string name; // inputName public string label; // etichetta del widget nel gruppo di stringhe pubbliche GUI; // gruppo del widget in GUIpublic string[] componentLabels; // per cursori (fino a 4 etichette) public string[] enumOptions; // per optionMenupublic InputPropertiesType type;public Vector4 maximum; // per cursori public Vector4 minimum; // per cursori public float step; // per cursori }public InputPropertiesType = 0,// 0 Float, // 1 Vector2, // 2 Vector3, // 3 Vector4, // 4 Color, // 5 Enum, // 6 Texture, // 7 String, // 8 Invalid = -1// -1 &rbrace;; | Nessuno |
| **bool** **Substance.Game.SubstanceGraph**.*HasInput*(**string** inputName) | Verifica se un input esiste in un grafico, restituisce true/false: | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |
| **bool** **Substance.Game.SubstanceGraph**.*IsInputVisible*(**string** inputName) | Verifica se un input visibleif è visibile, restituisce true/false | **Stringa** *nomeInput* Nome dell&#39;input nella SBSAR |

## Rendering in corso

| Public, metodo | Descrizione | Parametro |
| --- | --- | --- |
| **void** *QueueForRender*() pubblico | Aggiungi grafico Substance alla coda | Nessuno |
| ***mySubstance.**&#x200B;RenderAsync()* | Rendering asincrono di tutti i grafici della Substance in coda | Nessuno |
| ***mySubstance.**&#x200B;RenderSync()* | Rendering sincrono di tutti i grafici della Substance in coda | Nessuno |

## Scripting in modalità Editor:

Per rendere permanenti le modifiche dei grafici in modalità Editor, è necessario reimportare ogni Substance corrispondente. Questa operazione viene eseguita con la seguente funzione:

```
static void ReImportSubstance(Substance.Game.Substance pSubstance)

{



// Re-import Substance object:

SubstanceImporter importer = AssetImporter.GetAtPath(pSubstance.assetPath) as SubstanceImporter;

importer.CommitSubstanceToImporter(pSubstance); // plugin function

EditorUtility.SetDirty(importer);

importer.SaveAndReimport();



}
```


(con &quot;CommitSubstanceToImporter&quot;, una funzione di plug-in Substance: copia tutti i parametri grafici modificati e/o gli input nell’oggetto importatore Substance, che viene quindi serializzato su disco tramite il meccanismo di importazione di Unity)
