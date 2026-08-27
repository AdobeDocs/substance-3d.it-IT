---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/arnold/arnold-substance-painter.html"
breadcrumb-title: ''
description: Usa i modelli di output Substance Painter per il modulo di rendering Arnold con materiale aiStandard per il rendering basato su impostazioni fisiche.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Arnold > Arnold - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arnold - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 3%

---


# Arnold - Substance Painter

Substance Painter 2020.1 (6.1.0) viene fornito con [Modelli di output](https://experienceleague.adobe.com/it/docs/substance-3d-painter/using/getting-started/export/output-templates/export-presets) per Arnold utilizzando il [materiale aiStandard](https://docs.arnoldrenderer.com/display/A5AFMUG/Standard+Surface).

![](../../../assets/arnold-export.png){width="800px"}

## Arnold Standard Shader (Arnold 5 e superiore)

| Substance Painter esportazione | Arnold AiStandardSurface |
| --- | --- |
| BaseColor | Base/Colore |
| Ruvidità | Specular/Rugosità |
| Metallicità | Base/Metallicità |
| Normale | (**Maya**) Geometria/Mappatura rilievo/bump2d (da utilizzare come normali di Spazio tangente) (**3ds** **Max**) Bitmap → normale |
| Altezza | (**Maya**) Shader/spostamento di Spostamento (**3ds** **Max**) Modificatore oggetto → Proprietà di Arnold → Spostamento → Usa mappa |
| Con emissioni | Emissione/Colore (Peso Di Emissione = 1,0) |
| Livello di anisotropia (non incluso nel Modello di output Arnold predefinito) | (**Maya**) Rivestimento/Anisotropia (**3ds** **Max**) Rivestimento/Anisotropia |
| Livello di anisotropia (non incluso nel Modello di output Arnold predefinito) | (**Maya**) Pelo/Rotazione (**3ds** **Max**) Pelo/Rotazione |

>[!NOTE]
>
> Le mappe che rappresentano i dati dovranno essere interpretate correttamente. Per ulteriori informazioni, consultare la pagina [Gestione del colore](../../../renderers/color-management/color-management.md).
