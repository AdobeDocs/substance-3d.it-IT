---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-instance-definition-ue5.html"
breadcrumb-title: ''
description: Creazione di definizioni di istanze di materiale con i materiali delle Substance in Unreal Engine 5 per ottimizzare le prestazioni di rendering della GPU.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Instance Definition - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Definizione istanza materiale - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---


# Definizione istanza materiale - UE5

Potete utilizzare le istanze dei materiali UE5 con le Substance. In questo modo si salva un grande passaggio nel processo di rendering GPU non caricando nuovo materiale nel processo. È possibile creare un MID in fase di esecuzione o nell&#39;editor. Con la versione 5.0.0 è stato aggiunto il supporto completo per l’istanza del materiale.

## Creazione di un&#39;istanza di materiale nell&#39;editor

1. Fate clic con il pulsante destro del mouse sul materiale UE5 creato e scegliete &quot;Crea istanza materiale&quot;. In questo modo viene creato un materiale di istanza UE5.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-31-at-6-07-08-pm?$png$&jpegSize=300&wid=1472)
1. Fai clic con il pulsante destro del mouse sulla factory dell&#39;istanza di substance e scegli &quot;Crea un&#39;istanza del grafico&quot;. In questo modo viene creata un&#39;istanza del grafico e viene creato un altro materiale UE5. Eliminate il materiale UE5 appena creato poiché non verrà utilizzato.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-10-38-pm.png)
1. Fate doppio clic sull&#39;istanza di materiale creata nel passaggio 1 e abilitate i parametri Texture per tutte le mappe.
1. Impostate la texture sulla nuova texture INST creata dal punto 2. In questo modo si imposta l&#39;istanza del materiale per utilizzare le mappe di output della sostanza dal grafico dell&#39;istanza.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-13-18-pm.png)

Ora disponete di un&#39;istanza di materiale UE5 che utilizza un set specifico di texture Substance. Questo è un modo più ottimizzato di lavorare con più sostanze in un progetto UE5. Per informazioni su come creare un MID utilizzando blueprint, consultare questa pagina. [Blueprint(UE5): istanza di materiale dinamico](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
