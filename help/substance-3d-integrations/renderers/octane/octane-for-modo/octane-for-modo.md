---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/octane/octane-for-modo.html"
breadcrumb-title: ''
description: Utilizzate i materiali Substance con il modulo di rendering per ottani in MODO tramite i materiali Live DB e le configurazioni di output corrette.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Octane > Octane for MODO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ottano per MODO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Ottano per MODO

## Substance nel plug-in MODO

Gli output della Substance funzionano in modo nativo con Octane. Puoi utilizzare i seguenti output di Substance e configurazioni di effetti per i livelli di texture.

1. Crea una Substance>Texture>Crea Substance e imposta la modalità su Materiale irreale. L&#39;uso di materiale irreale consente di visualizzare la texture nella finestra della vista OGL avanzata.
1. Crea output per colore di base, metallizzato, rugosità e normale.
1. MODO utilizza le mappe Normale OGL. Nelle proprietà della Substance, è necessario modificare la direzione normale in OpenGL.

   ![](../../../assets/ogl.png)
1. Caricare il predefinito Substance PBR. Questo predefinito è una sostituzione di ottano. Trascinalo nel gruppo shader.

   [Substance\_PBR.lxp](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/integrations/files/162005234/162005272/1/1502792782697/substance-pbr.lxp)
1. Selezionate l&#39;esclusione e trascinate gli output della Substance dal Browser clip nella Vista schematica. Prendere il nodo con l&#39;output del nome file e collegarlo al nodo di input appropriato, ad esempio il colore di base → il colore di base.

   ![](../../../assets/connect-6.png)
1. Collegare le altre uscite della Substance

   ![](../../../assets/outputs-4.png){width="640px"}
