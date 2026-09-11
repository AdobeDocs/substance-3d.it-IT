---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: Esportate texture Substance Painter per il modulo di rendering Redshift utilizzando i modelli di output e le impostazioni del materiale corrette.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Redshift > Redshift - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Redshift - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---


# Redshift - Substance Painter

Substance Painter 2020.1 (6.1.0) supporta Redshift [Modelli di output](https://docs.substance3d.com/display/SPDOC/Export) per metallizzazione/rugosità (rsMaterial). Puoi semplicemente esportare utilizzando il modello Redshift per produrre texture compatibile con i materiali Redshift.

![](../../../assets/rs-export.png)

## Impostazione materiale Redshift

| Substance Painter esportazione | Materiale Redshift |
| --- | --- |
| Colora | Diffusa/Colore |
| Ruvidità | Riflessione/Rugosità (BRDF = GGX) |
| Metallicità | Riflesso/Metallicità (Tipo Fresco = Metallicità) |
| Normale | Complessivo / Mappa rilievo / rsBumpMap (Tipo mappa di input = Spazio tangente normale - Scala Height = 1,0) |
| DisplaceHeightField | Shader di Spostamento/rsDisplacement TexMap (codifica mappa = campo Height) |
| EmissionColor | Totale / Emissioni (Peso Delle Emissioni = 1,0) |

>[!NOTE]
>
> Le mappe che rappresentano i dati dovranno essere interpretate correttamente. Per ulteriori informazioni, consultare la pagina [Gestione del colore](../../../renderers/color-management/color-management.md).

## Esempio di Maya/Redshift

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
