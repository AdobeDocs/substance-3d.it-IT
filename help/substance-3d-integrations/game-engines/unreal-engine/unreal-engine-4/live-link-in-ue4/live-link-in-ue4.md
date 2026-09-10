---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/live-link-in-ue4.html"
breadcrumb-title: ''
description: Usa Live Link in Unreal Engine 4 per sincronizzare in tempo reale i materiali Substance tra Painter e UE4.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Live Link in UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Live Link in UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# Live Link in UE4

>[!WARNING]
>
> Live Link in Unreal Engine non è più supportato. Gli utenti con una versione precedente del plug-in in cui viene utilizzato Live Link potranno comunque utilizzare la funzione.

>[!WARNING]
>
> Live Link non funziona con trame BSP UE4. La risorsa che invii deve essere un file modello importato nel tuo progetto UE4

## Creazione del collegamento a Substance Painter

1. Apri Substance Painter
1. Fai clic con il pulsante destro del mouse sulla risorsa che desideri inviare a Painter nel Browser dei contenuti e scegli &quot;Invia a Painter&quot;.

   ![](../../../../assets/link1-22.png){width="400px"}
1. La trama verrà visualizzata in Substance Painter ed è possibile iniziare a creare texture. Mentre lavorate, le texture verranno inviate a UE4 e applicate ai materiali. Il punto verde sull’icona UE4 nella barra degli strumenti indica che il collegamento è dinamico e che si inviano texture.

   ![](../../../../assets/icon-12.png)

   1. Puoi mettere in pausa lo streaming di dati nelle opzioni Configura per il plug-in. Seleziona Plug-in>dcc-live-link e scegli Configura. Disattiva Abilita streaming per sospendere l&#39;invio di dati a UE4.

      ![](https://helpx-prod.scene7.com/is/image/HelpxProd/config-6?$png$&jpegSize=100&wid=393)
1. Le texture di Painter verranno visualizzate nel Browser contenuti e applicate al materiale in UE4.

   ![](../../../../assets/link3-11.png){width="500px"}
1. Un progetto Substance Painter (.spp) verrà creato nella cartella di progetto UE4 in una cartella denominata &quot;.sp&quot;

   ![](../../../../assets/link4-5.png)

## Ripristino di un collegamento a Substance Painter

Puoi riprendere da dove avevi interrotto dopo aver chiuso Painter o Unity.

1. Apri il progetto .spp in Substance Painter che si trova nella cartella Progetto Unity>risorse>.sp.
1. Fate clic con il pulsante destro del mouse sulla trama nel Browser contenuti e scegliete &quot;Invia a Painter&quot; per ristabilire il collegamento.

   ![](../../../../assets/link5-3.png){width="600px"}
