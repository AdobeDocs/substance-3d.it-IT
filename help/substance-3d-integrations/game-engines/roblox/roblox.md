---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/roblox.html"
breadcrumb-title: ''
description: Utilizza i materiali Substance in Roblox Studio con il flusso di lavoro Rugosità metallica PBR per esperienze 3D coinvolgenti.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Roblox
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Roblox
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# Roblox

[Roblox](https://www.roblox.com/) è una piattaforma per esperienze 3D coinvolgenti multiplayer. Roblox Studio, lo strumento di progettazione Roblox, supporta il flusso di lavoro Rugosità metallica PBR.

<table>
<tr style="border: 0;">
<td width="58.30%" style="border: 0;" valign="top">

## Modello Substance 3D Designer

Per creare texture per Roblox, puoi utilizzare il file Substance 3D seguente come modello [Substance grafici di composizione](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/substance-compositing-graphs) in [Substance 3D Designer](https://experienceleague.adobe.com/en/docs/substance-3d-designer/home).

[![Immagine dell&#39;icona del formato di file sbs collegata al modello roblox.](../../assets/sbs.png){width="64px"}](https://helpx.adobe.com/content/dam/roblox.sbs)

Questo modello di grafico consente la preconfigurazione dei nomi e dei tipi di file delle texture finali. Questo modello può essere installato e riutilizzato per creare nuovi materiali che seguono sempre le linee guida per i materiali Roblox.

</td>
<td width="41.60%" style="border: 0;" valign="top">

![](https://helpx-prod.scene7.com/is/image/HelpxProd/roblox-template?$png$&jpegSize=100&wid=401){width="200px"}

</td>
</tr>
</table>

## Flusso di lavoro da Designer a Roblox

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Installa modello

Per prima cosa, *installa* il modello Roblox.

* Scarica il file del modello collegato in precedenza.
* Vai alla directory dei documenti utente di Designer:
* (Creative Cloud desktop) `/Documents/Adobe/Adobe Substance 3D Designer`\
  (Vapore) `/Documents/Allegorithmic/Substance Designer/`
* Creare una cartella di modelli.
* Inserite il file in tale cartella.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-01-place-template.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Rileva modello

Quindi, chiedi a Designer di *guardare* la cartella dei modelli per cercare i modelli di grafico.

* In Designer, passa a **Modifica > Preferenze...**
* Nella finestra [Preferenze](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/preferences-window), vai a **Progetti > Progetto utente > Generali**
* Nell&#39;elenco **Directory modelli** fare clic sul pulsante **+**
* Passa alla directory `templates` e fai clic su **Seleziona cartella**
* Fai clic sul pulsante **OK**.
* Vai a **File > Nuovo > Substance grafico...**
* Verifica che il modello `Roblox` sia elencato nella parte inferiore dell&#39;elenco dei modelli nella finestra [Nuovo grafico Substance](https://helpx.adobe.com/substance-3d/unlisted/documentation/sddoc/create-a-graph-102400068.html)

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-02-detect-template.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Esporta texture

Create un grafico utilizzando il modello Roblox ed esportate le bitmap da quel grafico una volta terminato di lavorare su un materiale.

* Nella finestra [Nuovo grafico Substance](https://helpx.adobe.com/substance-3d/unlisted/documentation/sddoc/create-a-graph-102400068.html), selezionare il modello `Roblox`
* Imposta eventuali identificatori e altri parametri per il grafico e fai clic su **OK**
* Lavora sul tuo materiale nella [Visualizzazione grafico](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/graph-view/the-graph-view). Per iniziare a usare il flusso di lavoro, consulta [qui](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/getting-started/workflow-overview)
* Al termine, vai a **Strumenti > Esporta bitmap...** nella *barra degli strumenti* della visualizzazione Grafico
* Nella finestra [Esporta bitmap](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/exporting-bitmaps), imposta un percorso **Destinazione** valido, assicurati che *tutti* gli output siano *selezionati* e fai clic su **Esporta**
* Verifica che le texture siano esportate correttamente nel percorso **Destinazione**

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-03-export-textures.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Creare materiale in Roblox

In Roblox, create una Variante materiale e assegnate le texture esportate da Designer.

* Seleziona la scheda **Modello** e fai clic su **Gestione materiali**
* Selezionate un *modello di materiale* e fate clic sul pulsante **Crea variante**
* Nella finestra **Crea variante**, imposta un nome per il materiale
* Per *ogni canale di materiale*, fate clic sul pulsante **Importa** e selezionate la texture corrispondente esportata da Designer
* Fai clic su **Salva**

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-04-roblox-create-material.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Applicare il materiale

Utilizzare la nuova variante di materiale nella scena Roblox

* *Selezionate* qualsiasi parte o trama nella scena di Roblox
* In **Gestione materiali**, selezionate la *variante materiale* e fate clic sul pulsante **Applica alle parti selezionate**

>[!NOTE]
>
> Se il colore delle texture appare diverso in Roblox, controlla l&#39;attributo **Colore** nella categoria **Aspetto** nelle proprietà dell&#39;oggetto a cui viene applicata la Variante materiale e assicurati che sia impostato su *Bianco puro*, ovvero RGB (255, 255, 255), che è etichettato *Bianco istituzionale* in Roblox.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-05-roblox-apply-material.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Regolare la suddivisione in porzioni

La quantità di ripetizione del materiale su una superficie, ad esempio l&#39;affiancatura, può essere regolata in qualsiasi momento.

* In **Gestione materiali**, selezionate la *variante materiale* e fate clic sul pulsante **Modifica**
* Nella finestra **Modifica variante**, regola il valore della proprietà **Studs Per Tile** in **Additional**: un valore *lower* genera una ripetizione *more*

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-06-roblox-adjust-tiling.gif){width="512px"}

</td>
</tr>
</table>
