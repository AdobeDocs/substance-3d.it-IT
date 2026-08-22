---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/maxwell/maxwell-substance-painter.html"
breadcrumb-title: ''
description: Esportate le texture di Substance Painter per il modulo di rendering Maxwell utilizzando le impostazioni corrette per modelli di output e materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Maxwell > Maxwell - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maxwell - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Maxwell - Substance Painter

Substance Painter 2020.1 (6.1.0) supporta Maxwell [Modelli di output](https://experienceleague.adobe.com/it/docs/substance-3d-painter/using/getting-started/export/export) per metallizzazione/rugosità e specular/lucidità. Puoi semplicemente esportare usando il Modello di output Maxwell**.\
Maxwell 5.1.0** si integra con Substance Painter per importare facilmente texture e impostare automaticamente un materiale Maxwell.

## Esportazione di texture

Potete scegliere i Modelli di output Maxwell (Rugosità metallica) o Maxwell (Lucidità Specular) per esportare le texture per il rendering in Maxwell.

![](../../../assets/maxwell-output.png){width="500px"}

## Applicazione di texture in Maxwell

Potete usare l&#39;integrazione Substance Painter in Maxwell per creare automaticamente un materiale con le mappe esportate da Substance Painter applicata.\
Per iniziare, fai clic con il pulsante destro del mouse sull&#39;elenco dei materiali e scegli **Nuovo>Substance Painter**.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maxwell-painter?$png$&jpegSize=100&wid=413)

Individuate la posizione in cui avete esportato le texture delle Substance Painter e selezionate una delle mappe, ad esempio il colore di base. Quando fai clic su Apri, l&#39;integrazione creerà un nuovo materiale Maxwell con le mappe assegnate.\
Se avete esportato più set di texture da Substance Painter, l’integrazione utilizzerà la convenzione di denominazione della texture per assegnare mappe di texture corrispondenti.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/image-material?$png$&jpegSize=100&wid=620){width="600px"}

Puoi quindi assegnare il materiale alla risorsa nella scena.

![](../../../assets/assigned.png){width="500px"}

Tutti i materiali applicati mediante l’integrazione Substance Painter.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/materials-assigned?$pjpeg$&jpegSize=300&wid=1511){width="800px"}
