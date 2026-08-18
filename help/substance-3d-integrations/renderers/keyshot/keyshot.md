---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/keyshot.html"
breadcrumb-title: ''
description: Utilizza i materiali Substance nel modulo di rendering Keyshot per la visualizzazione del prodotto con le mappe delle texture esportate.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Keyshot
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Keyshot
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 8%

---


# Keyshot

*Keyshot 6.1.72*[&#x200B; Scarica Scena Di Esempio](https://www.dropbox.com/s/rvjsbbcx7c74aah/keyshot.zip?dl=0)

## Substance Painter esportazione

1. Per Keyshot, dovrete configurare un predefinito di esportazione utilizzando Diffusione, Riflessione, Metallico, Rugosità e Normale (X diretto).

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/key-01?$png$&jpegSize=300&wid=1794)

## Impostazione avanzata dei materiali

Userai 2 materiali avanzati. Uno sarà per il metallo e l&#39;altro sarà per il dielettrico.

1. Impostate il materiale su Avanzate e tracciate il grafico del materiale.

   **Metallico:**\
   a. Impostare Indice rifrazione su 10\
   b. Imposta le mappe come indicato nella tabella seguente

   | Substance Painter texture | Advanced Material Channel |
   | --- | --- |
   | Diffusione | Diffusione |
   | Metallizzato | Opacità |
   | Normale | Rilievo \*Normale attivato |
   | Ruvidità | Ruvidità |
   | Riflesso | Speculare |

1. Creare un nuovo materiale avanzato

   **Dielettrico:**\
   a. Impostare l&#39;indice di rifrazione su 1,5\
   b. Imposta le mappe come indicato nella tabella seguente

   | Substance Painter texture | Advanced Material Channel |
   | --- | --- |
   | Diffusione | Diffusione |
   | Normale | Rilievo \*Normale attivato |
   | Ruvidità | Ruvidità |
   | Riflesso | Speculare |

1. Prendete l&#39;output del materiale avanzato metallico e aggiungetelo al + del materiale avanzato dielettrico. In questo modo viene creato un campo Etichetta sul materiale.

   ![](../../assets/key-02.png)
