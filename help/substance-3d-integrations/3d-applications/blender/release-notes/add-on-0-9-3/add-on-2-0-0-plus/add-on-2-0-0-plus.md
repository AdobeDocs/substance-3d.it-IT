---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-3/add-on-2-0-0-plus.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il componente aggiuntivo Blender versione 2.0.0 e successive per scoprire le nuove funzioni e i miglioramenti.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 2.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Componente aggiuntivo 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---


# Componente aggiuntivo 2.0.0+

## Componente aggiuntivo 2.2

<b>Aggiunto:</b>

* Supporto per il modulo di rendering in ottano
* Supporto iniziale per Redshift
* Supporto iniziale per Renderman

<b>Aggiornato:</b>

* Aggiornamento alla versione più recente del connettore
* È stata aggiunta una funzionalità per ricevere i predefiniti tramite il connettore
* È stata migliorata la funzionalità di importazione predefinita: ora, tutte le istanze di una SBSAR che includono il materiale aggiungeranno il predefinito
* Funzionalità del connettore standardizzata

<b>Corretto:</b>

* Bug di persistenza in cui l&#39;immagine di input non funzionava dopo il salvataggio del file di fusione
* Problema con la rete di shader non funzionante quando si aggiorna il predefinito di shader
* URL errato nel pulsante del plug-in di download
* Affiancamento invertito in ottano
* Valori di input non funzionanti con renderer di terze parti
* Problema in cui non è stato creato il parametro del valore di input float
* Gli spazi colore di Renderman non funzionano correttamente
* I predefiniti di Shader non vengono filtrati in base al modulo di rendering disponibile

## Componente aggiuntivo 2.1.1

Questo aggiornamento include il supporto per Blender 4.0+ e diverse nuove funzioni nelle Preferenze di Componente aggiuntivo. Abbiamo inoltre aggiunto il supporto per Substance Connector per il trasferimento senza interruzioni di dati tra Substance 3D Sampler e Blender (Invia a) e risolto alcuni bug. Di seguito sono riportate le note dettagliate sulla versione.

<b>Aggiunto/Aggiornato:</b>

* È stata aggiunta la funzionalità del connettore Substance (supporta file SBSAR e file USD).
* Supporto per Blender 4.0+.
* Supporto per SRE versione 2.1.0.
* In Preferenze Componenti Aggiuntivi:
  * Possibilità di scegliere il percorso di installazione degli strumenti di integrazione delle Substance.
  * Pulsante per ripristinare il percorso predefinito degli Strumenti di integrazione.
  * pulsante per aprire la cartella Strumenti di integrazione.
  * Aggiunto Applica il tipo per assegnare il materiale (Inserisci: impostalo come materiale principale, Aggiungi: aggiungilo alla parte inferiore dell&#39;elenco).
  * Casella di controllo aggiunta per selezionare il comportamento predefinito dei gruppi di input (compressi/espansi).
  * È stata aggiunta una casella di controllo per selezionare il comportamento predefinito della proprietà Aggiorna solo texture.
  * Avvia automaticamente il motore remoto di Substance all’apertura del modulo di fusione (importante che sia abilitato se si utilizza Connettore).
* In Componente aggiuntivo:
  * Aggiunte solo le texture di aggiornamento (consente di modificare i parametri senza ricreare il grafico del nodo).
  * Sono stati aggiunti i pulsanti Espandi tutti i gruppi e Comprimi tutti i gruppi.
  * È stato aggiunto il gruppo Immagine di input per raggruppare tutte le immagini di input, se necessario in un SBSAR.
  * I parametri immessi vengono ora visualizzati nello stesso ordine di Designer.
  * È stata aggiunta l’anteprima con le miniature di ogni materiale Substance.

<b>Corretto:</b>

* È stato corretto un bug del gruppo di input Generale vuoto.

<b>Problemi noti:</b>

* La funzionalità di selezione automatica SBSAR durante la selezione di un oggetto al momento non funziona, quindi è disabilitata.

## Componente aggiuntivo 2.0.0

Substance 3D Addon 2.0 segna un aggiornamento trasformativo per gli utenti di Blender, con un&#39;architettura plug-in completamente refactoring. Questa riprogettazione si concentra su un&#39;integrazione senza interruzioni, prestazioni migliorate e una base flessibile per le espansioni future. Rappresenta non solo un aggiornamento, ma una reimmaginazione di come i materiali Substance vengono gestiti all&#39;interno di Blender, soddisfacendo le esigenze in evoluzione dei professionisti 3D.

<b>Aspetti salienti della versione 2.0:</b>

* Architettura con refactoring: struttura di plug-in migliorata per prestazioni e integrazione migliori
* Supporto per l’espansione futura: l’aggiornamento getta le basi per l’aggiunta semplice di nuove funzioni in futuro
* Compatibilità più ampia: completamente compatibile con Blender versione 3.0 e successive, incluso il supporto per gli utenti Mac

<b>Aggiunto/Aggiornato:</b>

* [SRE] Substance Engine il supporto per la selezione (GPU è l’impostazione predefinita)
* [SRE] Nuovi formati di immagine per esportare le texture
* [SRE] Profondità di bit la selezione per ogni tipo di mappa
* [BLD] Supporto per output di valore
* [BLD] Supporto input stringa
* [SRE] È stata aggiunta l’opzione per selezionare la cartella temporanea predefinita per la destinazione di esportazione delle immagini

<b>Corretto:</b>

* [SRE] Miglioramento generale delle prestazioni
* [BLD] Problemi di comunicazione risolti tra gli strumenti di integrazione e Blender
* [BLD] Impossibile installare/avviare gli strumenti di integrazione
* [BLD] Gli strumenti di integrazione non terminano quando si chiude Blender
* [BLD] Il materiale non si aggiorna quando si modifica il tipo di file di una mappa
* [SRE] Tutte le mappe dei materiali vengono esportate in qualsiasi momento
* [SRE] Gli strumenti di integrazione esportano mappe normali con scale
* [SRE] Il caricamento della Substance non termina mai
* [SRE] Le unità Dimensioni fisiche non vengono regolate in base alla scena
* [BLD] I predefiniti generati in Blender non funzionano con altre integrazioni
* [BLD] Il materiale non si aggiorna nei cicli
* [BLD] I limiti soft e hard degli input vengono ignorati
* [BLD] L’intensità del colore non si aggiorna correttamente quando si regola un parametro
* [SRE] La disinstallazione degli strumenti di integrazione non riesce
* [SRE] È stato risolto il problema a causa del quale la duplicazione di materiali più volte causava un errore.
* [SRE] Lo spazio colore dei nodi immagine ora corrisponde correttamente alle preferenze dell&#39;utente.

<b>Problemi noti:</b>

* Quando si utilizza Blender v4.0+, i socket non sono in ordine dopo aver attivato e disattivato più volte
* Cltr+Z per annullare le modifiche potrebbe causare errori
* Il caricamento di un file vuoto o di una cartella invece di un file .sbsar potrebbe interrompere il plug-in
* Supporto per la modalità headless di Blender
