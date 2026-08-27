---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/renderman/renderman-substance-painter.html"
breadcrumb-title: ''
description: Esporta le texture Substance Painter per Renderman utilizzando il materiale pxrSurface e le conversioni di output corrette.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Renderman > Renderman - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderman - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 1%

---


# Renderman - Substance Painter

Substance Painter 2020.1 (6.1.0) supporta [**pxrSurface**](https://rmanwiki.pixar.com/display/REN/PxrSurface) e [Modelli di output](https://docs.substance3d.com/display/SPDOC/Export) pxrDisney.

![](../../../assets/renderman.png)

Si consiglia di utilizzare **pxrSurface** per l&#39;output.

![](../../../assets/pxrsurface.png)

## Renderman Shader (Maya - RM 23.1)

| Substance Painter esportazione | PxrSurface |
| --- | --- |
| DiffuseColor | Diffusione/Colore |
| Rugosità speculare | Rugosità/Specular primario |
| SpecularFaceColor | Colore Specular/Volto Principale |
| Normale | Globali/rilievo/Orientamento → PxrNormalMap (Open GL) |
| Spostamento | (canale rosso ) PxrDispTransform (Risultato F) → (disp scalare) PxrDisplace (Colore di stacco) → (Shader di Spostamento) PxrSurfaceSG |
| GlowColor | Bagliore/Colore (Guadagno = 1,0) |
| Presenza | Globali/Presenza |

>[!NOTE]
>
> Le mappe che rappresentano i dati dovranno essere interpretate correttamente. Per ulteriori informazioni, consultare la pagina [Gestione del colore](../../../renderers/color-management/color-management.md).
