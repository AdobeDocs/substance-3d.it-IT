---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-2-0.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il plug-in Unity versione 2.2.0 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.2.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità 2.2.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Unità 2.2.0

## 2.2.0 Note sulla versione

**data di rilascio: 1/10/2019**

### Plug-in core:

* Versione di Substance Engine aggiornata
* Stabilità del codice migliorata
* **Supporto di Unity 2018.3**
* Supporto di **.NET 4.x**
* Supporto per Substance Source nel 2018.3
* Il problema di colorazione delle Substance Source è stato risolto
* Il grafico e il materiale corrispondente hanno ora lo stesso nome oggetto
* Sono stati aggiunti miglioramenti alla leggibilità dell’interfaccia grafica di Unity Pro
* Supporto aggiunto per le assegnazioni di output del materiale
* È stato corretto un bug nella gestione sRGB.
* È stato corretto un bug a causa del quale un utente poteva eliminare tutte le istanze di un grafico
* È stato corretto un bug a causa del quale il tentativo di eseguire il rendering della Substance durante la modifica dei parametri in fase di runtime poteva eseguire il rendering di due soli elementi alla volta.
* Quando si importa un pacchetto che contiene vecchi file di Substance, il plug-in ora comunica all&#39;utente che contiene vecchi dati di Substance e li elimina quando Unity sta tentando di importarli (in questo modo l&#39;utente non deve eliminare tutto manualmente se è danneggiato)
* È stato aggiunto il pulsante Informazioni su nel menu Substance per visualizzare le informazioni di compilazione relative al plug-in di Substance.
* Sono state aggiunte descrizioni del mouse nell’interfaccia grafica di Substance per visualizzare i nomi dei parametri Substance esposti
* Sono stati aggiunti dei pulsanti di navigazione nell&#39;interfaccia grafica della Substance per collegarla al grafico e ai materiali della Substance.
* Sono state aggiunte nuove icone per la Substance di grafici/materiali/texture nel Browser dei contenuti
* Le miniature delle Substance nel browser dei contenuti sono state aggiornate
* Rimosso il file .mat dalla parte anteriore dei nomi dei materiali della Substance
* È stata aggiunta la possibilità di rinominare grafici e materiali Substance
* Quando si modifica la risoluzione del grafico Substance, il popup di applicazione/ripristino non viene più visualizzato obbligando l’utente a confermare la modifica in quel momento
* È stato corretto un bug a causa del quale il processo Reflection utilizzava solo la risoluzione Substance predefinita, anziché quella definita dall’utente.
* È stato aggiunto un avviso di passaggio del mouse all’interfaccia utente della Substance che informa l’utente se lo spazio colore è impostato su Gamma
* Funzionalità modificata delle istanze del grafico a Substance: gli utenti possono ora creare istanze del grafico in una Substance senza che venga richiesto di specificare ogni istanza creata nell’interfaccia grafica del grafico a Substance

### Script:

* Sono state nascoste alcune funzioni non pensate per il supporto di script
* È stata aggiunta la funzione per duplicare le istanze del grafico a Substance tramite script: Duplicate()
* Funzione aggiunta per eseguire query sulle informazioni di input procedurali tramite C#, restituisce una matrice di elementi &#39;InputProperties&#39;: GetInputProperties()
* Funzione aggiunta per verificare se un input esiste in un grafico, restituisce true/false: HasInput(string inputName)
* È stata aggiunta una funzione per verificare se un input visibleif è visibile, restituisce true/false: IsInputVisible(string inputName)
* Lo schema di rendering è stato riprogettato. Di conseguenza, RenderSubstancesAsync() è stato dichiarato obsoleto ed è stato modificato in graphName.RenderAsync()

## Problemi noti:

**Plug-in Substance principale**

* L&#39;utente deve disabilitare &quot;Abilita codice di bit&quot; nel menu Impostazioni di compilazione in Xcode per generare per iOS
* Le anteprime degli oggetti Substance nel Browser contenuti vengono visualizzate in nero quando la destinazione di compilazione è impostata su Android/iOS
* Il pulsante di Alpha e il cursore di anteprima Mip Map (&lt;Mappa ip>) risultano mancanti sull’interfaccia grafica non Substance dopo l’importazione del plug-in Substance
* L’utente deve utilizzare i poteri di due per definire la risoluzione di un grafico a Substance tramite script
* I materiali Substance non sono persistenti quando vengono esportati/importati utilizzando un pacchetto Unity
* La Substance non funziona con Bundle risorse
* Le icone di anteprima della Substance nel Browser risorse vengono tutte modificate nell&#39;icona Substance S dopo una reimportazione
* Se si rinomina un grafico a Substance contenente un materiale, tale materiale verrà rimosso dagli oggetti a cui è applicato.
* (Solo Mac) L&#39;aggiornamento del plug-in su Mac rimuove i materiali delle Substance dai prefabbricati nella scena|

**Scripting**

* Lo scripting non funziona in fase di runtime se il progetto è impostato su x86 nelle impostazioni di compilazione
* Problemi con l’utilizzo del back-end di scripting il2cpp con determinate piattaforme di compilazione

**Substance Painter collegamento dinamico**

* La creazione di un progetto dopo aver colorato con Substance Live Link riporterà la trama dipinta a un materiale predefinito
* Canale AO non inviato con Painter Live Link
* Le trame con più materiali non funzionano in Unity Live Link
* Il modo in cui Unity LiveLink utilizza SimpleJson si scontra con altre istanze di SimpleJson in un progetto
