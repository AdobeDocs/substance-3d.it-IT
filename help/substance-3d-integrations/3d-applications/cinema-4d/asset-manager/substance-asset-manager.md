---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/substance-asset-manager.html"
breadcrumb-title: ''
description: Usa Substance Asset Manager in Cinema 4D per aggiungere, rimuovere e organizzare i materiali Substance nella scena.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Substance Asset Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestione risorse Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Gestione risorse Substance

Nella finestra Gestione risorse Substance sono elencate tutte le Substance caricate in una scena. Qui puoi aggiungere, rimuovere e riorganizzare la Substance.

Selezionando (clic sinistro) una Substance all’interno di Substance Asset Manager si apre la Substance in Gestione attributi di Cinema 4D. Lì puoi modificare i parametri e gli input della Substance dei fotogrammi chiave come qualsiasi altro parametro in Cinema 4D.

>[!NOTE]
>
> Gestione attributi dispone di una speciale modalità Risorse Substance, utile per avere un Gestione attributi dedicato per le Substance nel layout di Cinema 4D.

![](../../../assets/cinema-4d-4.png){width="500px"}

## Menu File

## Carica risorsa...

Carica una nuova Substance nella scena (come nel menu Plug-in).

Chiudi

Chiude Gestione risorse Substance. Le Substance cariche rimarranno naturalmente nella scena.

## Menu Modifica

## Seleziona tutte le Substance

Seleziona tutte le Substance elencate in Asset Manager. La stessa operazione può essere effettuata premendo Ctrl+a, mentre il mouse passa sopra Asset Manager.

## Deseleziona tutte le Substance

Deseleziona tutte le Substance elencate in Gestione risorse. Lo stesso si può ottenere premendo Maiusc+Ctrl+a, mentre il mouse passa il mouse sopra Gestione risorse.

## Seleziona da materiali selezionati

Seleziona tutte le Substance a cui fanno riferimento i materiali *selezionati*.

## Seleziona da materiali contrassegnati

Seleziona tutte le Substance a cui fanno riferimento i materiali *contrassegnati*. In Cinema 4D, un materiale viene contrassegnato se è selezionato un oggetto o un tag che utilizza questo materiale.

## Seleziona materiali

Seleziona tutti i materiali che fanno riferimento alle Substance selezionate.

## Menu Azioni

## Crea materiali

Crea nuovi materiali di Cinema 4D dalle Substance selezionate. I canali dei materiali verranno automaticamente inizializzati con gli shader di Substance che fanno riferimento ai rispettivi canali di output delle Substance.

## Duplica Substance/e

Duplica la Substance attualmente selezionata. Ciò può essere utile per utilizzare la stessa Substance con diversi set di parametri su più materiali.

## Reimporta Substance

Questa funzione può essere utilizzata per tornare ai valori predefiniti di una Substance o per integrare modifiche esterne (ad esempio, dal Substance Designer).\
Nota: **tutte** le modifiche apportate ai parametri negli input della Substance andranno perse.

## Rimuovi Substance

Rimuove dalla scena la Substance attualmente selezionata. Lo stesso si può ottenere premendo il tasto Canc mentre il mouse passa sopra Asset Manager.

## Elimina Substance inutilizzate

Rimuove tutte le Substance attualmente non referenziate da alcun materiale.

## Substance Engine menu

Il contenuto di questo menu dipende dal sistema operativo su cui è in esecuzione il Cinema 4D. La modifica della Substance Engine avrà effetto solo dopo il riavvio del Cinema 4D.

## Menu di scelta rapida

Facendo clic con il pulsante destro del mouse su una Substance selezionata, viene visualizzato il menu di scelta rapida. La loro funzionalità è identica a quella delle funzioni con lo stesso nome nei menu sopra citati:

* Rimuovi
* Crea materiali
* Duplica Substance
* Reimporta Substance
* Seleziona tutte le Substance
* Deseleziona tutte le Substance
* Seleziona materiali

## Trascina e rilascia

Puoi interagire con Substance Asset Manager tramite trascinamento. Sono disponibili diverse opzioni:

* Carica le Substance nella scena trascinandole da Esplora risorse o dal Finder e rilasciandole semplicemente su Gestione risorse Substance.
* Le Substance possono essere trascinate nel campo di collegamento degli shader di Substance per collegare uno shader e una risorsa di Substance.
* Se sei in modalità Non ordinato (vedi di seguito), puoi riorganizzare le Substance in Gestione risorse trascinandole in una nuova posizione.


## Ordinamento in Substance Asset Manager

## Modalità non ordinata

## Substance Asset Manager è in **modalità non ordinata per impostazione predefinita**. La cella dell&#39;intestazione della colonna del nome non contiene una freccia a destra. Puoi usare il trascinamento per riordinare le sostanze a tuo piacimento.

![](../../../assets/cinema-4d-3.png){width="500px"}

![](../../../assets/cinema-4d-5.png){width="500px"}

## Anteprime in Substance Asset Manager

## Substance Asset Manager visualizza icone piccole con anteprime dei canali disponibili per ciascuna Substance.

## Le anteprime vengono semplicemente visualizzate nell’ordine dei canali di output nella Substance. La colonna in cui viene visualizzata l&#39;anteprima non ha alcun significato.
