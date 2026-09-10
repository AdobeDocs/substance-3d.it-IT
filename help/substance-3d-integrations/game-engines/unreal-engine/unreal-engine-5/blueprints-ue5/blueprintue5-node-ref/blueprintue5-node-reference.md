---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-node-reference.html"
breadcrumb-title: ''
description: Guida di riferimento per tutti i nodi Substance Blueprint disponibili in Unreal Engine 5 per le operazioni sui materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Riferimento nodo Blueprint(UE5)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---


# Blueprint(UE5): riferimento nodo

## Nodi Substance generali:

| Nome | Input | Descrizione |
| --- | --- | --- |
| **GetSubstances** | Input: **Materiale** | Restituisce una matrice di istanze di Grafico Substance utilizzate da un materiale. Se create un materiale che utilizza output di texture da due diverse istanze di grafo, questa funzione restituirà queste due istanze di grafo. |
| **GetSubstanceTextures** | Input: **SubstanceGraphInstance** | Restituisce una matrice di tutte le texture abilitate e attualmente calcolate dal parametro di input Istanza di Grafico Substance. |
| **GetGraphName** | Input: **SubstanceGraphInstance** | Restituisce il nome del grafico impostato in Designer. |
| **GetFactoryName** | Input: **SubstanceGraphInstance** | Restituisce il nome della **GraphInstanceFactory** utilizzata per creare la **SubstanceGraphInstance** passata in questo nodo. |
| **GetSubstanceLoadingProgress** | NESSUNO | Restituisce un valore float compreso tra 0 e 1 con la percentuale di quante sostanze sono state completamente caricate. |
| **CreateGraphInstance** | Input: **SubstanceInstanceFactory** - Factory da cui si desidera creare un&#39;istanza del grafico.Input: **GraphIndex** (int) - Indice del grafico da creare. Input: **InstanceName** (FString) - Il nome che si desidera assegnare alla nuova istanza. | Restituisce una nuova istanza di grafico standalone che persisterà fino alla chiusura dell&#39;applicazione. |
| **DuplicateGraphInstance** | **SubstanceGraphInstance**: l&#39;istanza del grafico di cui si desidera creare una copia. | Restituisce una nuova istanza di grafico standalone che persisterà fino alla chiusura dell&#39;applicazione. |
| **EnableInstanceOutputs** | Input: **SubstanceGraphInstance** - Istanza del grafico contenente l&#39;output per abilitare Input: **OutputIndices** (matrice int32) - Indici degli output che si desidera abilitare. | Se precedentemente disattivato, vengono creati gli output di texture di **SubstanceGraphInstance** passati. Questa funzionalità ha la stessa funzionalità dell&#39;abilitazione dell&#39;output dall&#39;editor **SubstanceGraphInstance**. *NOTA: questa operazione non aggiornerà il materiale con la nuova texture creata. Questo problema deve essere gestito impostando un parametro di campionatore in fase di esecuzione utilizzando il nuovo output.* |
| **DisableInstanceOutputs** | Input: **SubstanceGraphInstance** - Istanza del grafico che contiene l&#39;output per disabilitare Input: **OutputIndices** (matrice int32) - Indici degli output che si desidera disabilitare | Se attivata, disattiverà ed eliminerà l’output della texture per l’oggetto grafico passato |
| **CopyInputParameters** | Input: **SubstanceGraphInstance** - Istanza del grafico a cui si desidera applicare valori Input: **SubstanceGraphInstance** - Istanza del grafico da cui si desidera ottenere i valori | Ripristina tutti i valori di input modificati del parametro di input Istanza di Grafico Substance. |
| **ResetInputParameters** | Input: SubstanceGraphInstance | Ripristinare i valori di input di un&#39;istanza di Grafico Substance sui valori predefiniti |
| **SetGraphInstanceOutputSize** | Input: **SubstanceGraphInstance** Input: Width - Texture Risoluzione della coordinata XInput: Height - Texture Risoluzione della coordinata Y | Imposta la risoluzione della texture di tutti gli output generati da questa istanza del grafico con le dimensioni passate dai parametri. Nota - Massimo 2048 su CPU EngineNota - Massimo 4096 su GPU Engine |
| **AsyncRendering** | **SubstanceGraphInstance** | Ricalcola le texture di output dell&#39;input dell&#39;istanza di Grafico Substance. (Non bloccante) |
| **SyncRendering** | **SubstanceGraphInstance** | Ricalcola le texture di output dell&#39;input dell&#39;istanza di Grafico Substance. (Blocco) |

## Funzioni specifiche dell&#39;istanza del grafico:

Può essere chiamato solo da un’istanza del grafico

| Nome | Input | Descrizione |
| --- | --- | --- |
| GetDynamicMaterialInstance | Input: Nome (stringa) | Restituisce l&#39;istanza del materiale dinamico di runtime di una sostanza o ne crea una se non esiste. Le istanze di materiale dinamico sono necessarie per la maggior parte delle modifiche dei valori di runtime dagli output dei valori di sostanza. |
| **GetInputNames** | NESSUNO | Restituisce una matrice di stringhe contenente tutti i nomi dei parametri di input. |
| **GetInputType** | NESSUNO | Restituisce il tipo di dati associato a questo input. |
| **SetInputInt** | Input: **Identificatore** (stringa)Input: **InputValues** (matrice int) | Modifica il valore di un input trovato dall&#39;Identificatore. Per poter applicare le modifiche, all&#39;interno di un gioco è necessario eseguire il rendering della sostanza utilizzando **AyncRender** o **SyncRender**. |
| **SetInputFloat** | Input: **Identificatore** (stringa)Input: **InputValues** (matrice float) | Modifica il valore di un input trovato dall&#39;Identificatore. Per poter applicare le modifiche, all&#39;interno di un gioco è necessario eseguire il rendering della sostanza utilizzando **AyncRender** o **SyncRender**. |
| **GetInputInt** | Input: **Identificatore** (stringa) | Restituisce una matrice di valori int con i valori correnti di un parametro di input. |
| **GetInputFloat** | Identificatore (stringa) | Restituisce una matrice di valori float con i valori correnti di un parametro di input. |
| **SetInputBool** | Input: **Bool** (booleano)Input: **Identificatore** (stringa) | Immette un valore booleano per assegnare un tipo di valore di input attivabile o disattivato. In precedenza, era possibile ottenere questo risultato solo impostando un valore int di 1 o 0 su una bool. |
| **GetInputBool** | Input: **Identificatore** (stringa) | Restituisce il valore booleano corrente di un input. |
| **SetIputColor** | Input: **Color** (LinearColor)Input: **Identifier** (FString) | Immette un valore FLinearColor a cui assegnare un tipo di valore di input del colore. In precedenza, questo era possibile solo impostando un valore float e passando una matrice di float. |
| **GetInputColor** | Input: Identificatore (FString) | Restituisce il valore del colore corrente in formato UE4. |
| **CreateAggregateSubstanceFactory** | Input: **Output Factory** (SubstanceInstanceFactory)*La fabbrica che crea gli output che verranno utilizzati come input per la fabbrica di input.* Input: **Output Factory Graph Index** (Integer)*Il grafico all&#39;interno della sostanza che si desidera utilizzare per combinare.* Input: **Input Factory** (SubstanceInputFactory)*La fabbrica che utilizza gli output come immagini di input dalla fabbrica di output.*Input:**Connections**(matrice di SubstanceConnections)*Questo può essere creato utilizzando il nodo blueprint Make Array. Per connessione Substance si intende il modo in cui è possibile creare il nodo di aggregazione che consente di collegare gli output.* **&#x200B; Return (SubstanceInstanceFactory)***Può essere utilizzato per creare un&#39;istanza del grafico della nuova istanza combinata.* | Il nuovo nodo della sostanza aggregata consente di prendere due factory dell&#39;istanza della sostanza e creare una nuova factory dell&#39;istanza in fase di esecuzione, che può essere utilizzata per creare una nuova istanza del grafico. Ciò che rende speciale questa operazione è che potete connettere le texture di output da una delle istanze del grafico combinato alle immagini di input dell’altra istanza del grafico combinato. Per creare un&#39;istanza del grafico Substance da questa nuova fabbrica, consulta la nostra documentazione sulle istanze del grafico runtime. |
| **SubstanceConnectionStruct** | Input: **Identificatore output** (FString)*Identificatore dell&#39;output della texture da concatenare in un input.* Input: **Identificatore di input** (FString) | Utilizzata da Create Aggregate Substance Factory per specificare come concatenare ogni texture di output con nuove texture di input. |
