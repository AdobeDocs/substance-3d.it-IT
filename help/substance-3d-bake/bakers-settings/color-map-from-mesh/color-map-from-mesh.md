---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: Proietta le proprietà dei colori dalle trame ad alto poli alle texture per eseguire i baking ID di polipinto o materiale per le maschere di selezione.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mappa colori da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 4%

---


# Mappa colori da trama

Questa Mappa colore da baker trama proietta le proprietà del colore da una trama ad alta definizione in una texture. Può essere utilizzato per eseguire i baking ID di poligono o materiale per creare maschere di selezione.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Origine colore** | Determina su quale proprietà della trama ad alto poli deve essere basata la generazione del colore.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Colore vertice</strong>: legge il colore del vertice e lo salva nella texture. I colori vengono interpolati da un vertice all’altro.</li><li data-preserve-html="true"><strong>Colore materiale</strong>: legge il colore del materiale assegnato a una faccia poligonale.</li><li data-preserve-html="true"><strong>ID trama</strong>: assegnate un colore per ogni oggetto trovato.</li><li data-preserve-html="true"><strong>ID sottogruppo/sottogruppo</strong>: assegnare un colore per sottooggetto (detto anche elemento).</li></ul> |
| **Generatore colori** | Definisce la modalità di generazione del colore quando **Origine colore** è impostato su **ID trama** o **ID poligruppo/subtrama**.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Casuale</strong>: ogni oggetto o sottooggetto è colorato con un colore generato in modo casuale.</li><li data-preserve-html="true"><strong>Scostamento tonalità</strong>: ogni oggetto o sottooggetto è colorato da un colore univoco basato su una tonalità.</li><li data-preserve-html="true"><strong>Scala di grigi</strong>: ogni oggetto o sottooggetto è colorato con un valore di scala di grigi univoco.</li></ul> |
