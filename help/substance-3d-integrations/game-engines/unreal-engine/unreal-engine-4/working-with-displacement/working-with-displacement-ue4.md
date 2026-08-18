---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: Abilita la tassellatura e utilizza le mappe di spostamento dai materiali delle Substance in Unreal Engine 4 per i dettagli della superficie.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Displacement - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo dello Spostamento - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Utilizzo dello Spostamento - UE4

Per lavorare con lo spostamento, dovrete attivare la tassellatura sul materiale.

![](../../../../assets/tess.png){width="600px"}

Per utilizzare l&#39;output di height, è necessario fare doppio clic sull&#39;output nell&#39;istanza di Substance Factory per creare il height. Height non è attivato per impostazione predefinita. Puoi quindi trascinare questo output di height nel materiale.

![](../../../../assets/height-1.png){width="800px"}

Una volta aggiunto l&#39;output del height al materiale, dovrete creare alcuni nodi per attivare il modificatore Spostamento mondiale e tassellatura.

1. Create 2 parametri scalari. Una sarà Distanza e l&#39;altra sarà il moltiplicatore per la tassellatura.
1. Moltiplica il canale Rosso dal Height al parametro Distanza
1. Aggiungere un nodo VertexNormalWS e moltiplicarlo con l&#39;output del multiplo nel passaggio 2.
1. Immettere la moltiplicazione di VertexNormal per lo Spostamento mondiale sul materiale.
1. Prendere il parametro del moltiplicatore di tassellatura e inserirlo nel moltiplicatore di tassellatura sul materiale.

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> Gli altri output di texture sono stati omessi in questa immagine per semplificare il grafico. Qui vengono mostrati solo i nodi Spostamento e Moltiplicatore per maggiore chiarezza.
