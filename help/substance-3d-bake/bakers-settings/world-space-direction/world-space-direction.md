---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: Calcola le direzioni vettoriali nello spazio mondo e salvale nelle texture per ottenere effetti direzionali e maschere.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Direction
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Direzione spazio globale
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 4%

---


# Direzione spazio globale

Il fornaio World Space Direction consente di calcolare una direzione vettoriale nello spazio mondiale in una texture.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Direzione di input** | Definisce l&#39;input da cui viene calcolata la direzione.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Da texture</strong>: la direzione del vettore è definita da una texture di input.</li><li data-preserve-html="true"><strong>Da vettore uniforme</strong> (impostazione predefinita): la direzione del vettore è definita dai cursori X, Y, Z.</li></ul> |
| **Orientamento normale** | Definisce se il formato normale della texture di output. Questo inverte il canale verde a seconda del formato.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> (impostazione predefinita)</li></ul> |
| **X Y Z** | Cursori per definire i 3 componenti del vettore di direzione, se **Direzione di input** è impostato su **Da vettore uniforme**. |
| **File di direzione** | Percorso del file di texture di input per definire il vettore di direzione, se **Direzione di input** è impostato su **Da texture**. |
