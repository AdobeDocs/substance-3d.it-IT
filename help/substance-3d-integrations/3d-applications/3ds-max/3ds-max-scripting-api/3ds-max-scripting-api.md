---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-scripting-api.html"
breadcrumb-title: ''
description: Documentazione di riferimento per l’API di scripting Substance 3ds Max per automatizzare le operazioni sui materiali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds MAX Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API di scripting per MAX 3ds
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 2%

---


# API di scripting per MAX 3ds

Di seguito è riportato l&#39;elenco dei comandi e delle proprietà per il nodo Substance 2.

## Proprietà:

| Proprietà | Descrizione | Tipo |
| --- | --- | --- |
| nome | Nome del nodo Substance2. L&#39;impostazione predefinita è &quot;Substance 2&quot; | Stringa |

## Comandi:

| Comando | Descrizione | Ritorno | Tipo restituito: | Parametro |
| --- | --- | --- | --- | --- |
| getCurrentPackageName | Ottiene il nome del file di base del pacchetto caricato (file sbsar caricato nel nodo del grafico) | Il nome file (senza la directory di prefissaggio) del pacchetto caricato (file sbsar) | Stringa |  |
| getCurrentGraphName | Ottieni il nome del grafico corrente | identificatore dell’istanza del grafico corrente | Stringa |  |
| getOutputsNamesFromCurrentGraph | Ottieni l’elenco dei nomi di utilizzo degli output abilitati | Tabella contenente l&#39;elenco dei nomi dei canali per gli output abilitati | Elenco |  |
| getPresetIdentifiers | Ottieni l’elenco dei predefiniti dal grafico della Substance | Tabella contenente l’elenco degli identificatori di stringa per tutti i predefiniti | Elenco |  |
| setPackageAndGraphNames | Caricare un file sbsar dal disco nel nodo grafico | Vero in caso di successo, falso in caso di fallimento | Booleano | ***Parametro stringa***: **substancePackageFilePath** Percorso del file sbsar nel parametro disk ***String***: **graphInstanceNameToSelect** Identificatore stringa del grafico |
| setInputInt | Imposta un input intero con un nuovo valore |  |  | ***Parametro Integer***: **valore** Valore Integer per impostare l&#39;input su ***parametro String***: **inputIdentifier** Identificatore di stringa univoco dell&#39;input |
| setInputFloat | Impostare un input a virgola mobile con un nuovo valore |  |  | ***Parametro float***: **valore** Valore float per impostare l&#39;input su ***parametro String***: **inputIdentifier** Identificatore di stringa univoco dell&#39;input |
| setInputString | Impostare un input stringa con un nuovo valore |  |  | ***Parametro stringa***: **valore** Valore stringa per impostare l&#39;input su ***Parametro stringa***: **inputIdentifier** Identificatore stringa univoco dell&#39;input |
| setInputBool | Impostare un input booleano con un nuovo valore |  |  | ***Parametro booleano:* valore &#x200B;** Valore booleano per impostare l&#39;input sul parametro&#x200B;***String &#x200B;***: **inputIdentifier** Identificatore di stringa univoco dell&#39;input |
| setInputVec2 | Impostare un input vettoriale con due elementi |  |  | Parametro ***Point2:**&#x200B;***valore** Valore massimo point2 per impostare l&#39;input sul parametro ***String &#x200B;***: **inputIdentifier** Identificatore di stringa univoco dell&#39;input |
| setInputVec3 | Impostare un input vettoriale con tre elementi |  |  | ***Parametro Point3:* valore &#x200B;** Valore massimo point3 per impostare l&#39;input su&#x200B;***parametro String &#x200B;***: **inputIdentifier** Identificatore di stringa univoco dell&#39;input |
| setInputVec4 | Impostare un input vettoriale con quattro elementi |  |  | ***Parametro Point4***: **valore** Valore massimo point4 per impostare l&#39;input su ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| setInputColor | Impostare un input colore con un nuovo valore |  |  | ***Parametro colore***: **valore** Valore colore massimo per impostare l&#39;input su ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| setInputComboSelection | Impostare il valore attualmente selezionato in un input casella combinata |  |  | ***Parametro Integer***: **valore** Indice del widget della casella combinata ***parametro String***: **inputIdentifier** Identificatore di stringa univoco dell&#39;input |
| getInputInt | Ottiene il valore di input per un tipo di input integer | Valore intero corrente dell&#39;input | Intero | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputFloat | Ottiene il valore di input per un tipo di input float | Valore a virgola mobile corrente dell&#39;input | A virgola mobile | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputString | Ottiene il valore di input per un tipo di input stringa | Valore stringa corrente dell&#39;input | Stringa | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputBool | Ottiene il valore di input per un tipo di input booleano | Valore booleano corrente dell&#39;input | Booleano | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputVec2 | Ottiene il valore di input per un tipo di input point2 | Il valore massimo corrente del punto2 dell&#39;input | Punto2 | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputVec3 | Ottiene il valore di input per un tipo di input point3 | Valore massimo corrente di punto3 dell&#39;input | Punto 3 | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputVec4 | Ottiene il valore di input per un tipo di input point4 | Valore massimo corrente del punto4 dell&#39;input | Punto4 | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputColor | Ottenere il valore di input per un tipo di input colore | Valore corrente dell&#39;input come colore | Colora | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getInputComboSelection | Ottiene l&#39;indice della selezione della casella combinata in base all&#39;identificatore | Indice dell&#39;elemento della casella combinata selezionato | Intero | ***Parametro stringa:* inputIdentifier &#x200B;** Identificatore stringa univoco dell&#39;input |
| getMaterialDependentCount | Ottieni il numero di dipendenze del materiale | Numero di riferimenti dipendenti di un tipo di materiale | Intero |  |
| ApplyValuesToSelectedPreset | Sostituisce il predefinito attualmente selezionato con i valori di input correnti |  |  |  |
| RemoveAllPresets | Rimuovi tutti i predefiniti nel nodo del grafico corrente. |  |  |  |
| CreatePreset | Crea un nuovo predefinito dagli input correnti |  |  | ***Parametro stringa:* newPresetName &#x200B;** Nome visualizzato per il nuovo predefinito |
| RemoveOnePreset | Rimuovi il predefinito con il nome specificato |  |  | ***Parametro stringa:* selectedPresetName &#x200B;** Nome del predefinito da rimuovere |
| ImportPreset | Importare il file sbsprs nei predefiniti correnti |  |  | ***String, parametro:**&#x200B;***filePath**, stringa contenente il percorso del file da cui importare il predefinito |
| ExportPreset&#x200B;**\*deprecato** Per rimuovere in 2.5.0\* | Esporta il predefinito attualmente selezionato in un file sbsprs |  |  | ***Parametro stringa***: **percorsoFile** Stringa contenente il percorso del file in cui esportare il predefinito |
| exportPresetList | Esporta i predefiniti specificati in un singolo file di predefiniti |  |  | ***Parametro stringa***: **percorsoFile** Stringa contenente il percorso del file per esportare i predefiniti nel parametro ***List***: **predefiniti** Elenco contenente i nomi dei predefiniti da esportare |
| BakeOutputsOfSelectedGraph | Eseguire i baking su disco le bitmap dell’istanza del grafico selezionata |  |  | ***Parametro stringa:* filePath &#x200B;** Directory del percorso principale in cui scrivere le immagini&#x200B;***Parametro stringa &#x200B;***: **imageFormatExtension** Estensione/formato del file in cui scrivere le immagini |
