---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: Genera texture di curvatura accurate da trame ad alto poli utilizzando il ray tracing per un rilevamento preciso dei bordi.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Curvatura da trama
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Curvatura da trama

La curvatura da fornaio trama genera una texture di curvatura da trame ad alto poli. È più lento della base [curvatura](../../bakers-settings/curvature/curvature.md) del fornaio, ma produce risultati più precisi.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Raggi secondari** | Quantità di raggi emessi per leggere la geometria circostante. Un valore elevato produce meno rumore ma richiede più tempo per il calcolo. Il valore predefinito è 32. |
| **Raggio di campionamento** | Misura in cui viene presa in considerazione la geometria vicina per calcolare la curvatura alla superficie della geometria. Valori alti possono produrre bordi più netti, mentre valori più bassi possono produrre bordi più sottili ma senza fornire alcuna informazione. |
| **Rispetto Al Rettangolo Di Selezione** | Definisce se il raggio di campionamento è relativo alla dimensione della trama o se è definito come una distanza basata su unità. |
| **Autointersezione** | Corrispondenza per nome dei raggi di curvatura. Indica in che modo i forni devono corrispondere alla geometria bassa e alta. Può essere utilizzato per filtrare il processo di cottura al forno senza la necessità di spostare manualmente (esplodere) le trame.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (impostazione predefinita): la trama a basso poli corrisponde a ogni trama a elevato poli.</li><li data-preserve-html="true"><strong>Per nome trama</strong>: filtrate le trame in base al nome per evitare che corrispondano a geometria indesiderata.</li></ul>Per ulteriori informazioni sulla geometria corrispondente, vedere: [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md). |
| **Limiti mappatura automatica dei toni** | Controlla la modalità di scrittura dei valori di curvatura nella texture. Se questa opzione è attivata, l’intervallo di valori verrà normalizzato tra 0 e 1 in base ai valori minimo e massimo rilevati durante il processo di esegue i baking. Se è deselezionata, i valori minimo e massimo vengono definiti manualmente.  **Nota:** quando si eseguono i baking UDIM/Porzioni UV, questo parametro deve essere disabilitato per rendere la mappatura tonale uniforme e non specifica per ogni porzione, altrimenti si potrebbero creare giunture tra ogni texture. Per trovare manualmente i giusti valori min/max, esegue i baking prima con questa impostazione attivata, quindi dai un&#39;occhiata alla console/registro per vedere quali valori sono stati generati dal baker. |
| **Tonemapping min** | Se **Limiti di mappatura tonale automatica** è disattivato, definisce il valore minimo per ridimensionare il risultato di curvatura in modo che si adatti alla texture. |
| **Tonemapping massimo** | Se **Limiti di mappatura tonale automatica** è disattivato, definisce il valore massimo per ridimensionare il risultato di curvatura in modo che si adatti alla texture. |
| **Mappa normale** | Percorso facoltativo di una texture normale. Può essere usato per sostituire il calcolo interno del fornaio. |
| **Spazio Mondiale** | Se questa opzione è attivata, la texture normale viene interpretata come una normale spazio mondo anziché come uno spazio tangente. |
| **Orientamento normale** | Formato della texture Normale se in Spazio tangente.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (impostazione predefinita)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
