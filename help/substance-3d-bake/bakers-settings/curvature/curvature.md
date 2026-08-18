---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: Estrai le informazioni di curvatura dalla trama per creare texture che evidenzino le cavità e i bordi della geometria.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Curvatura
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%

---


# Curvatura

Il fornaio curvatura consente di estrarre una texture di curvatura. Questa texture contiene informazioni su cavità e spigoli relative alla geometria.

Le proprietà della texture sono definite come:

* I valori del nero rappresentano aree concave.
* I valori bianchi rappresentano aree convesse.
* I valori di grigio rappresentano aree neutre (principalmente piatte).

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Algoritmo** | Definisce la modalità di calcolo delle informazioni di curvatura sulla trama. |
| **Dettagli** | Controlla l’intensità delle informazioni nella curvatura. Un valore elevato può produrre più dettagli ma meno dettagli. |
| **Abilita giunture** | Se questa opzione è attivata, il fornaio tenterà di ridurre le giunture tra le Isole UV copiando i testi ai bordi da un lato all’altro. |
| **Cuciture** **Intensità** | Se **Abilita giunture** è abilitato, questo parametro controlla la forza della giuntura. |
