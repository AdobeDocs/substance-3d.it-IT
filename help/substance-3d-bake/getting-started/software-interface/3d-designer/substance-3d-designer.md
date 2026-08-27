---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/getting-started/software-interface/substance-3d-designer.html"
breadcrumb-title: ''
description: Scoprite come accedere e utilizzare la finestra di esegue i baking in Substance 3D Designer per eseguire i baking le informazioni sul modello in texture.
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

### Elemento da Eseguire i baking

![](../../../assets/sd-mesh-selection.png)

Questo pannello controlla quale parte della trama a basso poli verrà utilizzata per la cottura al forno.

Questo pannello elenca la geometria trovata all&#39;interno del file mesh low-poly. Per impostazione predefinita, l’elenco si basa sui singoli materiali presenti nel file, ma può essere sostituito da sottoreti, se necessario. Potete deselezionare gli elementi che devono essere ignorati durante il processo di cottura al forno.

### Output

![](../../../assets/sd-output.png)

Questo pannello controlla la posizione della texture cotta.

| *Parametro* | *Descrizione* |
| --- | --- |
| **Metodo** | Controlla come verranno memorizzate le texture cotte con la confezione di Substance.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Embedded</strong>: la texture baked è memorizzata in una sottocartella accanto al pacchetto Substance con un nome specifico.</li><li data-preserve-html="true"><strong>Collegata</strong> (impostazione predefinita): la texture eseguita i baking viene archiviata nella cartella definita e quindi viene fatto riferimento alla Substance inserita nel pacchetto.</li></ul> |
| **Cartella** | Posizione delle texture eseguite i baking al momento del salvataggio. Fai clic sul pulsante con tre punti per aprire una finestra di dialogo e scegli la cartella di esportazione. A destra sarà visibile un segno di spunta che indica se la cartella esiste effettivamente o meno. |
| **Nome** | Convenzione di denominazione delle texture eseguite i baking. Fate clic sul pulsante con tre punti per aprire un menu a discesa e inserire altri segnaposto (nome di backup, personalizzato, materiale, trama). |
| **Esempio** | Simulare un nome di file per verificare la convenzione di denominazione. |
| **Inserire la risorsa in una cartella specifica della trama** | Se questa opzione è attivata, le texture eseguite i baking verranno salvate in una cartella denominata file mesh. |

### Trame ad alta definizione

![](../../../assets/sd-high.png)

Questo pannello controlla l’elenco delle trame a poli alti e le relative impostazioni. Per ulteriori informazioni, vedere [parametri comuni](../../../bakers-settings/common-parameters/common-parameters.md).

### Valori predefiniti

![](../../../assets/sd-default-values.png)

Per ulteriori informazioni, vedere [parametri comuni](../../../bakers-settings/common-parameters/common-parameters.md).

### Elenco baker e impostazioni

![](../../../assets/sd-baker-list.png)

Il baker è il punto in cui potete scegliere quale texture eseguita i baking generare. Per impostazione predefinita, l’elenco è vuoto.

* **Aggiunta nuovo baker:** Fare clic sul pulsante &quot;Aggiungi Baker&quot;.
* **Rimozione di un baker:** Selezionare il baker nell&#39;elenco, quindi fare clic sul pulsante &quot;Elimina baker&quot;.
* **Spostamento di un baker all&#39;inizio:** Selezionare il baker nell&#39;elenco, quindi fare clic sul pulsante &quot;Pull to top&quot;.
* **Spostamento verso il basso di un baker:**&#x200B;selezionare il baker nell&#39;elenco, quindi fare clic sul pulsante &quot;Premere verso il basso&quot;.

Per impostazione predefinita, ogni baker nell’area eredita i valori predefiniti (vedi sopra). È possibile, ad esempio, ignorare le dimensioni (risoluzione) facendo clic sulla cella sulla riga del baker. Questo vale per le altre impostazioni della riga.

Quando si fa clic su un baker nell&#39;elenco, la vista Parametri Baker viene aggiornata con i relativi parametri specifici.

Per ulteriori informazioni sui parametri specifici, vedere: [Impostazioni Baker](../../../bakers-settings/bakers-settings.md).
