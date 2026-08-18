---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-4.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.3.4 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.3.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Unità 2.3.4

>[!WARNING]
>
> **L&#39;utilizzo del plug-in con Unity 2019.2 produrrà il seguente errore:**
> 
> InspectorSubstanceImporter.OnInspectorGUI deve chiamare ApplyRevertGUI per evitare comportamenti imprevisti.\
> UnityEditor.Experimental.AssetImporters.AssetImporterEditor:OnDisable()\
> Substance.Editor.InspectorSubstanceImporter:OnDisable()
> 
> Questo errore può essere cancellato e non influirà sulla funzionalità del plug-in

>[!WARNING]
>
> **Leggere: Substance interruzione materiali:**\
> I materiali di Substance che contengono un output personalizzato con un utilizzo vuoto verranno interrotti durante l&#39;importazione. Inoltre, i materiali di Substance contenenti usi duplicati si interromperanno.\
> I file sbsar precedenti di GameTextures.com non sono attualmente compatibili con la Substance nel plug-in Unity. Questi materiali che contengono output di utilizzo non supportati sono danneggiati. Prima di utilizzare il plug-in, assicurati di creare un backup del progetto.

## Nuove funzioni:

* Supporto aggiuntivo per Substance Engine v7
* Aggiunto supporto Linux

### Correzioni di bug:

* Risolti i problemi relativi all’importazione di una Substance senza mappe texture
* È stato risolto un problema per cui il processo di riflessione non funzionava correttamente in Unity 2019.x
* Risolti i problemi di gestione dei prefabbricati durante l’importazione di un pacchetto contenente prefabbricati con materiali Substance
* Assegnazioni di materiali/texture fisse non riportate dopo il processo di riflessione
* È stato risolto un problema relativo alla modifica degli ombreggiatori che causava l’interruzione dei materiali
* È stato risolto un problema a causa del quale la rugosità non veniva imballata nel canale alfa metallico.
* È stato risolto un problema a causa del quale, quando era installato il plug-in Substance, la modifica delle impostazioni di importazione per le texture non sostanziali annullava alcune opzioni.
* È stato risolto un problema che impediva l’apertura della Substance Source in Mac.

## Problemi noti:

**Plug-in Substance principale**

* L&#39;utente deve disabilitare &quot;Abilita codice di bit&quot; nel menu Impostazioni di compilazione in Xcode per generare per iOS
* La Substance non funziona con Bundle risorse
* Le icone di anteprima della Substance nel Browser risorse vengono tutte modificate nell&#39;icona Substance S dopo una reimportazione
* I materiali di Substance personalizzati con un output con utilizzo impostato su vuoto interromperanno il materiale
* I materiali di Substance personalizzati che hanno usi duplicati interromperanno il materiale
* L&#39;editor deve essere riavviato dopo l&#39;importazione del plug-in in Linux

**Scripting**

* Lo scripting non funziona in fase di runtime se il progetto è impostato su x86 nelle impostazioni di compilazione
* Problemi con l’utilizzo del back-end di scripting il2cpp con determinate piattaforme di compilazione

**Substance Painter collegamento dinamico**

* La creazione di un progetto dopo aver colorato con Substance Live Link riporterà la trama dipinta a un materiale predefinito
* Canale AO non inviato con Painter Live Link
* Le trame con più materiali non funzionano in Unity Live Link
* Il modo in cui Unity LiveLink utilizza SimpleJson si scontra con altre istanze di SimpleJson in un progetto
