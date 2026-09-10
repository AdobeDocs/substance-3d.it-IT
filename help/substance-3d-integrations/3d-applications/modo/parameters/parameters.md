---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/parameters.html"
breadcrumb-title: ''
description: Modificate i parametri dei materiali Substance in MODO tramite il pannello Proprietà Substance per personalizzare i materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parametri
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# Parametri

Una Substance ha un insieme di parametri principali. Questi parametri sono suddivisi in Substance, Output e Modifiche. Sono disponibili nel pannello Proprietà Substance.\
La Substance da Substance Source conterrà i parametri tecnici e i canali. Le opzioni Canale non hanno alcun effetto in MODO. Gli output vengono attivati/disattivati utilizzando la sezione Output.

![](../../../assets/parameters-4.png){width="300px"}

## Substance

Una Substance ha un set di parametri principali, che si trovano nella categoria Substance del pannello Proprietà Substance.

* **Ricarica Substance:** Questo parametro consente di ricaricare una Substance. È stato progettato per essere utilizzato con Substance Designer. Se state lavorando su una Substance personalizzata e avete aggiunto una nuova modifica o un nuovo output, potete ricaricare la Substance appena pubblicata in MODO. Le nuove modifiche e gli output verranno aggiunti e le impostazioni di modifica precedenti rimarranno invariate.
* **Modalità di Ombreggiatura:** Questi parametri consentono di impostare la modalità di ombreggiatura da utilizzare per la Substance. Princippled (predefinito), Unreal, Unity o glTF.
* **Ripristina Substance:** Questo parametro ripristinerà le modifiche alle impostazioni predefinite.
* **Seleziona grafico:** consente di scegliere il grafico nel file di Substance dal quale creare un materiale.
* **Carica predefinito:** È possibile caricare un predefinito, che configurerà i parametri di modifica della Substance. I predefiniti possono essere creati con Substance Player. Il file predefinito è di tipo .sbsprs. Una volta caricato un predefinito, è necessario fare clic sul menu a discesa Predefinito e scegliere il predefinito, in quanto .sbsprs può contenere diversi predefiniti.
* **Salva predefinito:** consente di salvare un predefinito
* **Seleziona predefinito:** consente di scegliere un predefinito incorporato nel file di Substance o dai predefiniti salvati in MODO.
* **Esegue i baking su disco:** Questo parametro esegue i baking le texture generate dalla Substance in un file bitmap.
* **Dimensione output:** Questo parametro ridimensionerà dinamicamente la texture in base alle dimensioni impostate. La Substance Engine rigenererà la texture alla dimensione desiderata.
* **Numero casuale:** Questo parametro varia la generazione procedurale della Substance. Questo parametro è ideale per la creazione di una versione casuale della stessa Substance. Consente di variare rapidamente i parametri della Substance per generare una nuova versione della texture

## Output

Le opzioni Output consentono di attivare o disattivare gli output della Substance. Un output è ciò che viene generato dalla Substance Engine e sottoposto a rendering come texture nell’albero degli Shader.

![](../../../assets/outputs-02.png){width="300px"}

## Modifiche

Le modifiche sono parametri creati nel file di Substance e modificabili in MODO. Puoi selezionare i canali e in modalità Articolo usa Cala canali per ottenere i controlli insieme in un controller popup.

![](../../../assets/haul.png){width="300px"}
