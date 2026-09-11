---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/toolbag.html"
breadcrumb-title: ''
description: Usa la rugosità delle Substance e gli output metallici in Toolbag 2 per l’anteprima e il rendering del materiale in tempo reale.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Toolbag
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toolbag
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 5%

---


# Toolbag

In questa pagina viene illustrato come utilizzare la rugosità/output metallico per Toolbag 2.

Toolbag supporta sia i flussi di lavoro specular/lucentezza che metallico/rugosità.

Per impostazione predefinita, Substance 3D Painter usa lo shader metallico PBR, ma potete usarlo anche con lo specular/lucentezza shader. Questo flusso di lavoro mostrerà come utilizzare gli output metallici per Toolbag 2. Toolbag supporta il flusso di lavoro metallico.

[Scarica scena di esempio](https://www.dropbox.com/s/qyed3un2zhtuibj/toolbag.zip?dl=0)

## Esportare da Painter

1. Quando si utilizza lo shader PBR metallico predefinito, è possibile esportare utilizzando i canali del documento predefiniti + Normale + Predefinito di esportazione AO.  ***\*La Mappa normale di esportazione dei canali dei documenti viene esportata in base alla configurazione del progetto. Toolbag richiede Mappa normale OGL. È possibile cambiare il formato normale nella configurazione del progetto.***
1. In alternativa, puoi creare una configurazione di esportazione personalizzata che utilizza lucentezze

   ![](../../assets/settings-export.png){width="600px"}
1. Prima dell’esportazione, potete impostare il formato normale su OpenGL.  **Modifica>Configurazione progetto**

   ![](../../assets/settings-normal-format.png)

## Impostazione materiale

1. Imposta Riflettività su Metallicità
1. Imposta Riflessione su GGX
1. Aggiungi le texture ai canali appropriati, come illustrato nel seguente grafico:

   | Substance 3D Painter Texture | Spazio colore | Materiale Toolbag |
   | --- | --- | --- |
   | Colore di base | sRGB | Albedo |
   | Ruvidità | sRGB disattivato | Microsuperficie - Lucentezza - Clic su Inverti |
   | Metallizzato | sRGB disattivato | Riflettività - Mappa metalness |
   | Normale | sRGB disattivato | Normale |
   | Occlusione ambientale | sRGB disattivato | Occlusione |

![](../../assets/settings-toolbag.jpg){width="600px"}
