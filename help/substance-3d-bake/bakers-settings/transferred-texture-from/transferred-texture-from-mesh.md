---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
breadcrumb-title: ''
description: Trasferisci texture tra trame in base ai loro UV, incluso il supporto per le conversioni delle mappe normali.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Transferred Texture from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texture trasferita da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 3%

---


# Texture trasferita da trama

Il baker di Texture trasferita da trama consente di convertire una texture da una trama all&#39;altra in base ai rispettivi UV. Questo baker supporta anche il trasferimento o le mappe normali (che richiedono conversioni speciali). Per funzionare, entrambe le trame necessitano di definizioni UV.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Texture file** | Percorso del file di texture di input che verrà trasferito. |
| **Set UV** | Trama UV da utilizzare sulla trama ad alto poli per leggere la texture e proiettarla sulla trama a basso poli. |
| **Modalità di filtro** | Definisce la modalità di interpolazione dei pixel della texture.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Più vicino</strong>: nessuna interpolazione. Utilizzare il pixel più vicino trovato in una determinata posizione. Preciso ma che può creare aliasing.</li><li data-preserve-html="true"><strong>Bilineare</strong> (impostazione predefinita): utilizzate i quattro pixel più vicini a una determinata posizione. Nessun alias ma può essere sfocato.</li></ul> |
| **Mappa normale** | Se attivata, indica al baker che la texture di input da trasferire è una mappa normale. Indica il baker per applicare conversioni speciali alla texture per renderla compatibile con la trama di destinazione. |
| **Tipo mappa** | Definisce il tipo di mappa normale della texture di input.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Spazio Mondiale</strong></li><li data-preserve-html="true"><strong>Spazio tangente</strong> (impostazione predefinita)</li></ul> |
| **Orientamento normale** | Definisce il formato normale della texture di input se **Tipo mappa** è impostato su **Spazio tangente**.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> (impostazione predefinita)</li></ul> |
