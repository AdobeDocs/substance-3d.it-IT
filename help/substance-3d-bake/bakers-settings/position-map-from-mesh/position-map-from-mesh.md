---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/position-map-from-mesh.html"
breadcrumb-title: ''
description: Calcola mappe di posizione accurate da trame ad alto poli per acquisire informazioni precise sulla posizione della geometria.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mappa posizione da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Mappa posizione da trama

La mappa di posizione dal fornaio trama calcola la posizione della geometria della trama ad alto poli e la salva in una texture. È simile al fornello in posizione base ma può produrre risultati più precisi.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Modalità** | Controlla quali informazioni verranno calcolate nella texture di posizione.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Tutti gli assi:</strong> trasforma la posizione degli assi X, Y e Z nei canali RGB della texture di output.</li><li data-preserve-html="true"><strong>Un asse:</strong> inserisce un singolo asse nella texture di output come immagine in scala di grigio.</li></ul> |
| **Asse** | Definisce l&#39;asse da calcolare se il parametro **Mode** è impostato su **One axis**. |
| **Tipo di normalizzazione** | Definisce come ridimensionare i valori di posizione per asse.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Box:</strong> normalizza ciascun asse in base al volume della trama (lunghezza del rettangolo di selezione).</li><li data-preserve-html="true"><strong>BSphere:</strong> normalizza tutti gli assi in base al raggio del volume della trama (sfera di delimitazione).</li></ul> |
| **Scala di normalizzazione** | Definisce come ridimensionare i valori di posizione in base alla trama.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Per materiale</strong>: i valori vengono ridimensionati in modo da essere compresi tra 0 e 1 per ogni materiale (set di texture).</li><li data-preserve-html="true"><strong>Scena completa</strong> (impostazione predefinita): i valori vengono ridimensionati in modo da tenere conto dell&#39;intera trama. Ciò consente di posizionare in modo continuo i valori tra oggetti e materiali (insiemi di texture).</li></ul> |
