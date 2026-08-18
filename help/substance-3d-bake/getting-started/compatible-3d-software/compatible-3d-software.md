---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Scopri quale software 3D è compatibile con Substance Bakers e come preparare trame per risultati di cottura ottimali.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Software 3D compatibile
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---


# Software 3D compatibile

La maggior parte dei software 3D è compatibile con Substance Baker a condizione che esportino la geometria mesh come poligoni nei formati di file supportati dalle applicazioni.

Tuttavia, non tutti i software sono allo stesso livello in termini di funzionalità e qualità durante l&#39;esportazione di queste trame. Per questo è importante pulire correttamente una rete e assicurarsi che sia compatibile con i forni. Per ulteriori informazioni su come preparare una trama, consultate le varie [Guide](../../guides/performances-and-opt/performances-and-optimizations.md).

## Compatibilità software

Di seguito è riportato un elenco dei software 3D più diffusi e la loro compatibilità con i panettieri:

| *Nome* | *Stato* |
| --- | --- |
| **Blender** | Compatibile: richiede di convertire i modificatori prima di esportarli. |
| **Maya** | Compatibile: richiede una cronologia di trasformazione bloccata ed eliminazione prima dell’esportazione. |
| **3DS max** | Compatibile: richiede una xForm reimpostata prima dell&#39;esportazione. |
| **MODO** | Compatibile: si consiglia di utilizzare il modulo di esportazione Game Tab impostato su &quot;Unreal Static Mesh&quot;. |
| **Cinema 4D** | Compatibile: richiede di convertire i modificatori prima di esportarli. |
| **zBrush** | Non compatibile: le trame a basso contenuto di poli devono prima essere elaborate e pulite in un’altra applicazione 3D. Compatibile: trame ad alto poli per la cottura al forno. |

## Formato file

Quando si esegue il baking della geometria, è importante tenere conto anche del formato di file utilizzato. Il formato di file definirà la quantità di informazioni che verranno salvate nella trama.

Troppe informazioni a volte possono essere dannose e causare errori. Di solito consigliamo di provare formati di file diversi quando si verificano errori, in quanto può essere un modo semplice per risolvere i problemi e determinare se il colpevole è nel fornaio stesso o proviene dal software 3D.

Di seguito è riportata una rapida panoramica dei due formati di file più comuni supportati dai forni:

| Formato file | Informazioni |
| --- | --- |
| **FBX** | Autodesk FBX (Filmbox) è il formato di file principale utilizzato da Autodesk Software, può essere scritto come testo o binario.  Essa sostiene:<ul data-preserve-html="true"><li data-preserve-html="true">UV (set multipli)</li><li data-preserve-html="true">Vertice, tangente e binomio</li><li data-preserve-html="true">Colori vertice</li><li data-preserve-html="true">Faccia triangolare, faccia quadrata e faccia N-Gon</li><li data-preserve-html="true">Fotocamere</li><li data-preserve-html="true">Luci</li><li data-preserve-html="true">Suddivisione delle maglie</li><li data-preserve-html="true">Gruppi di arrotondamento</li><li data-preserve-html="true">Informazioni sul materiale (come il colore)</li><li data-preserve-html="true">Bitmap</li></ul> |
| **OBJ** | Wavefront OBJ è un formato di file basato su testo molto semplice che supporta:<ul data-preserve-html="true"><li data-preserve-html="true">UV (un solo set)</li><li data-preserve-html="true">Normali vertici</li><li data-preserve-html="true">Colori vertice (solo se esportato da Pixologic zBrush)</li><li data-preserve-html="true">Faccia triangolare, faccia quadrata e faccia N-Gon</li><li data-preserve-html="true">Colore materiale (se è presente un file <strong>mtl</strong>)</li></ul> |
