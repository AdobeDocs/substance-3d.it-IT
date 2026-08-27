---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: Scopri come utilizzare il fornaio di Occlusione ambiente per generare texture di ombre ambiente utilizzando algoritmi con accelerazione GPU.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Occlusione ambientale
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 4%

---


# Occlusione ambientale

Il fornaio con Occlusione ambiente consente di creare una texture di ombra ambientale. Questo baker utilizza un algoritmo veloce eseguito sulla GPU.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit

>[!WARNING]
>
> * Questo baker potrebbe non essere supportato con le vecchie GPU.
> * La cottura ad alta risoluzione su GPU di fascia bassa/mobili può causare un arresto anomalo.

## Parametri

| *Nome* | *Descrizione* |
| --- | --- |
| **Mappa normale** | Inserire un file di mappa normale che può essere utilizzato per fornire ulteriori dettagli geometrici sulla superficie della trama da prendere in considerazione durante il calcolo del fornaio. Questo parametro è facoltativo. |
| **Spazio Mondiale** | Se questa opzione è attivata, specificate che la mappa normale di input si trova nello spazio globale (anziché nello spazio tangente). Se non viene fornita alcuna mappa normale di input, questi parametri vengono ignorati/disabilitati. |
| **Inverti normale** | Calcola la mappa di occlusione ambientale con le normali invertite (può essere utilizzata per generare una mappa di thickness). |
| **Usa parti trama non selezionate** | Utilizzate le parti di trama non selezionate della trama per creare la mappa di occlusione ambientale. |
| **Qualità** | Scegli la qualità della mappa di Occlusione ambientale. Una qualità superiore è più lenta da calcolare.Valori disponibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bassa</strong> (3 passaggi)</li><li data-preserve-html="true"><strong>Media</strong> (impostazione predefinita, 5 passaggi)</li><li data-preserve-html="true"><strong>Alto</strong> (10 passaggi)</li><li data-preserve-html="true"><strong>Altissima</strong> (16 passaggi)</li></ul> |
| **Distinzione precisione** | Precisione dell&#39;occlusione ambiente. Un valore più basso fornisce una precisione maggiore, ma può produrre artefatti più grandi. |
| **Dissolvenza distanza** | Estensione dell&#39;occlusione ambientale. |
