---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: Genera mappe di spessore colando i raggi verso l'interno dalle superfici mesh per utilizzarli negli shader SSS e nella mascheratura.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Thickness Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mappa spessore da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 5%

---


# Mappa spessore da trama

La mappa di spessore da trama è molto simile al baker di occlusione ambientale, ma proietta i raggi dalla superficie della trama all&#39;interno. Questa texture può essere utilizzata in uno shader di dispersione delle superfici secondarie (SSS) o per texture di mascheramento.

Le proprietà della texture sono definite come segue:

* I valori di nero rappresentano le parti sottili del modello.
* I valori bianchi rappresentano le parti spesse del modello.

**Disponibile in:**

* Substance Painter
* Substance Designer
* Substance Automation Toolkit

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Raggi secondari** | Quantità di raggi di occlusione. Un valore elevato produce meno rumore ma richiede più tempo per il calcolo. Il valore predefinito è 64. |
| **Distanza minima occlusione** | Distanza minima alla quale i raggi di occlusione colpiscono la geometria poly elevata. Il valore predefinito è 0,00001. |
| **Distanza massima occlusione** | Distanza massima alla quale i raggi di occlusione colpiscono la geometria poly elevata. Il valore predefinito è 0,1. |
| **Rispetto al rettangolo di selezione** | Se questa opzione è attivata, le unità sono relative al rettangolo di selezione dell’oggetto (1,0 è la lunghezza diagonale del rettangolo di selezione). Se è disattivata, le unità utilizzate per le distanze minime e massime dell’occluder sono quelle definite durante l’esportazione della trama (metri, centimetri o qualsiasi unità sia la scena esportata). |
| **Angolo di diffusione** | Angolo di estensione massimo dei raggi di occlusione. Il valore predefinito è 180. |
| **Distribuzione** | Distribuzione angolare dei raggi di occlusione.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Coseno</strong> (impostazione predefinita)</li><li data-preserve-html="true"><strong>Uniforme</strong></li></ul> |
| **Ignora carattere di sfondo** | Se questa opzione è attivata, i raggi di occlusione ignorano i colpi su una superficie posteriore (se la normale poly alta è orientata in direzione opposta a quella del poly basso da cui viene sparato il raggio). Nella maggior parte dei casi questa impostazione deve essere abilitata per evitare artefatti. |
| **Occlusione autonoma** | Corrispondenza del nome per i raggi di occlusione. Indica in che modo i forni devono corrispondere alla geometria bassa e alta. Può essere utilizzato per filtrare il processo di cottura al forno senza la necessità di spostare manualmente (esplodere) le trame.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (impostazione predefinita): la trama a basso poli corrisponde a ogni trama a elevato poli.</li><li data-preserve-html="true"><strong>Per nome trama</strong>: filtrate le trame in base al nome per evitare che corrispondano a geometria indesiderata.</li></ul>Per ulteriori informazioni sulla geometria corrispondente, vedere: [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md). |
| **Normalizzazione automatica** | Definisce se i valori di output devono essere ridimensionati per adattarsi a un intervallo compreso tra 0 e 1 (il punto più chiaro è impostato sul bianco puro e il punto più scuro sul nero puro). |
