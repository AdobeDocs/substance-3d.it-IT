---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers.html"
breadcrumb-title: ''
description: Utilizza i materiali Substance con i principali moduli di rendering come Arnold, V-Ray, Redshift e altri nel tuo flusso di lavoro 3D.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Moduli di rendering
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 1%

---


# Moduli di rendering

I materiali Substance forniti in [Substance Source](https://source.substance3d.com/) contengono output per shader basati su dati fisici e supportano sia il [flusso di lavoro Metallico/Rugosità (flusso di lavoro predefinito) che il flusso di lavoro Specular/Lucentezza](https://academy.substance3d.com/courses/pbrguides). È importante comprendere il flusso di lavoro supportato dal materiale di rendering. A seconda del modulo di rendering, potresti essere in grado di utilizzare direttamente gli output di materiale Substance o potresti dover convertire le texture di output. I materiali di Substance personalizzati o che scarichi dal Substance share potrebbero non contenere gli output appropriati necessari per un determinato modulo di rendering.

![](../assets/outputs.png){width="200px"}

Ad esempio, con Arnold o Vray Next, potete utilizzare direttamente output metallizzati/di rugosità. Tuttavia, con la funzione pxrSurface di Renderman, gli output metallizzati/di colore di base devono essere convertiti in colori diffusi e specular del volto. Un plug-in di integrazione Substance gestirà automaticamente queste conversioni se il modulo di rendering è supportato.

Con Substance Painter, puoi scegliere un [Modello di output](https://experienceleague.adobe.com/it/docs/substance-3d-painter/using/getting-started/export/export-window/export-window) che creerà i tipi di mappa appropriati necessari per un determinato modulo di rendering. Se il modulo di rendering non è supportato per impostazione predefinita, puoi anche creare Modelli di output personalizzati.

**Substance Painter Modello di output**

![](../assets/output-template.png){width="500px"}

## Guide per il rendering

* [Conversione delle uscite Substance](../renderers/converting-outputs/converting-substance-outputs.md)
* [Gestione colore](../renderers/color-management/color-management.md)
* [Arnold](../renderers/arnold/arnold.md)
* [Vray](../renderers/vray/vray.md)
* [Renderman](../renderers/renderman/renderman.md)
* [Redshift](../renderers/redshift/redshift.md)
* [Maxwell](../renderers/maxwell/maxwell.md)
* [Corona](../renderers/corona/corona.md)
* [Ottano](../renderers/octane/octane.md)
* [Keyshot](../renderers/keyshot/keyshot.md)
* [Thea](../renderers/thea/thea.md)
* [Maverick](../renderers/maverick/maverick.md)
* [Toolbag](../renderers/toolbag/toolbag.md)
* [Cicli ed eventi](../renderers/cycles-and-eevee/cycles-and-eevee.md)
