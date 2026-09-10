---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: Calcola texture normali incurvate che descrivono la direzione media dell'illuminazione ambientale da trame ad alto poli.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Normali incurvate da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 3%

---


# Normali incurvate da trama

Il baker Normali incurvate da trama calcola una texture che descrive la direzione media dell&#39;illuminazione ambientale. Questo baker deriva dall&#39;Occlusione ambientale [dal baker Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md).

**Disponibile in:**

* Painter
* Designer
* Toolkit di automazione

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Raggi secondari** | Quantità di raggi di occlusione. Un valore elevato produce meno rumore ma richiede più tempo per il calcolo. |
| **Distanza minima occlusione** | Distanza minima in cui i raggi di occlusione colpiranno la geometria poly alta&#x200B;**.** |
| **Distanza massima occlusione** | Distanza massima alla quale i raggi di occlusione colpiscono la geometria poly elevata. |
| **Rispetto al rettangolo di selezione** | Se questa opzione è attivata, i calcoli della distanza dei raggi sono basati sullo spazio normalizzato (da 0 a 1) della trama a basso poli. Se è disattivata, il calcolo della distanza del raggio si basa sulle unità specificate nella trama a basso poli al momento dell’esportazione (metri, centimetri, ecc.). |
| **Angolo di diffusione** | Angolo di estensione massimo dei raggi di occlusione. Il valore predefinito è 180. |
| **Distribuzione** | Distribuzione angolare dei raggi di occlusione.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Coseno</strong> (impostazione predefinita)</li><li data-preserve-html="true"><strong>Uniforme</strong></li></ul> |
| **Ignora carattere di sfondo** | Se questa opzione è attivata, i raggi di occlusione ignorano i colpi su una superficie posteriore (se la normale poly alta è orientata in direzione opposta a quella del poly basso da cui viene sparato il raggio). Nella maggior parte dei casi questa impostazione deve essere abilitata per evitare artefatti. |
| **Occlusione autonoma** | Corrispondenza del nome per i raggi di occlusione. Indica in che modo i forni devono corrispondere alla geometria bassa e alta. Può essere utilizzato per filtrare il processo di cottura al forno senza la necessità di spostare manualmente (esplodere) le trame.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (impostazione predefinita): la trama a basso poli corrisponde a ogni trama a elevato poli.</li><li data-preserve-html="true"><strong>Per nome trama</strong>: filtrate le trame in base al nome per evitare che corrispondano a geometria indesiderata.</li></ul>Per ulteriori informazioni sulla geometria corrispondente, vedere: [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md). |
| **Tipo mappa** | Definisce il tipo di texture di output.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Spazio globale</strong></li><li data-preserve-html="true"><strong>Spazio tangente</strong> (impostazione predefinita)</li></ul> |
| **Orientamento normale** | Controlla il formato normale della texture di output se **Mat Type** è impostato su Spazio tangente.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong> (impostazione predefinita)<strong> <br/></strong></li></ul> |
