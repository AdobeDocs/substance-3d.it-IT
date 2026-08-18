---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/getting-started/software-interface/substance-3d-designer.html"
breadcrumb-title: ''
description: Scoprite come utilizzare la finestra di cottura in Substance 3D Designer per inserire le informazioni sul modello nelle texture.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Software Interface > Substance 3D Designer
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Designer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 2%

---


# Substance 3D Designer

![](../../../assets/sd-mesh-right-click.png)

È possibile accedere alla finestra di cottura tramite il file mesh nella finestra [Esplora risorse](https://helpx.adobe.com/it/substance-3d/unlisted/documentation/sddoc/the-explorer-129368147.html). Fate clic con il pulsante destro del mouse sul nome della trama e scegliete &quot;**Informazioni sul modello di forno**&quot; per aprire la finestra di cottura al forno.

## Panoramica

![](../../../assets/sd-window-overview.png){width="500px"}

La finestra di cottura di è divisa in diversi pannelli che sono descritti di seguito.

### Elemento da cuocere

![](../../../assets/sd-mesh-selection.png)

Questo pannello controlla quale parte della trama a basso poli verrà utilizzata per la cottura al forno.

Questo pannello elenca la geometria trovata all&#39;interno del file mesh low-poly. Per impostazione predefinita, l’elenco si basa sui singoli materiali presenti nel file, ma può essere sostituito da sottoreti, se necessario. Potete deselezionare gli elementi che devono essere ignorati durante il processo di cottura al forno.

### Output

![](../../../assets/sd-output.png)

Questo pannello controlla la posizione della texture cotta.

| *Parametro* | *Descrizione* |
| --- | --- |
| **Metodo** | Controlla come verranno memorizzate le texture cotte con la confezione di Substance.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Embedded</strong>: la texture baked è memorizzata in una sottocartella accanto al pacchetto Substance con un nome specifico.</li><li data-preserve-html="true"><strong>Collegata</strong> (impostazione predefinita): la texture in baked viene memorizzata nella cartella definita e quindi referenziata nella Substance collocata.</li></ul> |
| **Cartella** | Posizione delle texture al forno quando vengono salvate. Fai clic sul pulsante con tre punti per aprire una finestra di dialogo e scegli la cartella di esportazione. A destra sarà visibile un segno di spunta che indica se la cartella esiste effettivamente o meno. |
| **Nome** | Convenzione di denominazione delle texture cotte. Fate clic sul pulsante con tre punti per aprire un menu a discesa e inserire altri segnaposto (nome di backup, personalizzato, materiale, trama). |
| **Esempio** | Simulare un nome di file per verificare la convenzione di denominazione. |
| **Inserire la risorsa in una cartella specifica della trama** | Se questa opzione è attivata, le texture al forno vengono salvate all’interno di una cartella denominata file mesh. |

### Trame ad alta definizione

![](../../../assets/sd-high.png)

Questo pannello controlla l’elenco delle trame a poli alti e le relative impostazioni. Per ulteriori informazioni, vedere [parametri comuni](../../../bakers-settings/common-parameters/common-parameters.md).

### Valori predefiniti

![](../../../assets/sd-default-values.png)

Per ulteriori informazioni, vedere [parametri comuni](../../../bakers-settings/common-parameters/common-parameters.md).

### Elenco dei forni e impostazioni

![](../../../assets/sd-baker-list.png)

Il fornaio è il punto in cui potete scegliere quale texture al forno generare. Per impostazione predefinita, l’elenco è vuoto.

* **Aggiunta di un nuovo fornaio:** Fare clic sul pulsante &quot;Aggiungi fornaio&quot;.
* **Rimozione di un fornaio:** Selezionare il fornaio nell&#39;elenco, quindi fare clic sul pulsante &quot;Elimina fornaio&quot;.
* **Spostamento di un fornaio in alto:** Selezionare il fornaio nell&#39;elenco, quindi fare clic sul pulsante &quot;Tirare in alto&quot;.
* **Spostare un fornaio verso il basso:**&#x200B;selezionare il fornaio nell&#39;elenco, quindi fare clic sul pulsante &quot;Spingere verso il basso&quot;.

Per impostazione predefinita, ogni baker eredita i Valori predefiniti (vedere sopra). Le dimensioni (risoluzione), ad esempio, possono essere sostituite facendo clic sulla cella sulla linea del fornaio. Questo vale per le altre impostazioni della riga.

Quando si fa clic su un fornaio nell&#39;elenco, la vista Parametri fornaio viene aggiornata con i relativi parametri specifici.

Per ulteriori informazioni sui parametri specifici, vedere: [Impostazioni dei forni](../../../bakers-settings/bakers-settings.md).
