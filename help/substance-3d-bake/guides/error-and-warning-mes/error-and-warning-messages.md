---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/error-and-warning-messages.html"
breadcrumb-title: ''
description: Guida di riferimento per tutti i messaggi di errore e di avvertenza che possono apparire durante la cottura con il software Substance.
helpx_creative_field: ""
helpx_description: bakers > Guides > Error and Warning Messages
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Messaggi di errore e di avvertenza
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Messaggi di errore e di avvertenza

Di seguito è riportato l’elenco di tutti i messaggi di errore che possono essere visualizzati durante la cottura al forno con software Substance.

## Qualsiasi panettiere

| *Messaggio* | *Descrizione* |
| --- | --- |
| Baker non disponibile. | Questo messaggio di errore è generalmente seguito da messaggi di errore aggiuntivi, spesso correlati a problemi della GPU. Può accadere se la GPU è troppo datata e non soddisfa i [requisiti tecnici](https://www.allegorithmic.com/products/tech-specs) del software. |
| Il set UV [X] non esiste. | Il Baker cercò di lavorare con un determinato set UV che non è presente nella trama a basso poli. |
| Impossibile caricare la scena dall&#39;URL. | Questo messaggio indica che il fornaio non è stato in grado di caricare il file mesh, di solito la mesh poly alta. Questo messaggio può essere originato da alcuni motivi:<ul data-preserve-html="true"><li data-preserve-html="true">Il file mesh a cui si fa riferimento non esiste più.</li><li data-preserve-html="true">Il file mesh è danneggiato o interrotto e non può essere letto.</li><li data-preserve-html="true">La trama è attualmente in fase di modifica da un&#39;altra applicazione e non può essere letta.</li></ul> |

## UV per SVG Baker

| *Messaggio* | *Descrizione* |
| --- | --- |
| Impossibile trovare UV per la trama [nome trama]. | Non sono stati trovati UV relativi a una trama specifica. Questo può accadere se vengono importate più trame, ma solo alcune di esse hanno UV. |
| La scena non ha UV. Annullamento del forno. | Se nella scena non è presente alcuna trama con UV, il processo di cottura al forno viene annullato. |

## Posizione Baker

| *Messaggio* | *Descrizione* |
| --- | --- |
| La trama [nome trama] non ha posizioni. | La trama poly bassa non ha posizioni di vertice. |
| La trama [nome trama] non contiene UV per l&#39;insieme UV [X]. | Il Baker cercò di lavorare con un determinato set UV che non è presente nella trama a basso poli. |

## Qualsiasi fornaio &quot;dalla trama&quot;

| *Messaggio* | *Descrizione* |
| --- | --- |
| Impossibile trovare le normali dei vertici nella trama [nome trama]. | Non sono stati trovati valori normali dei vertici nella mesh specificata. Normalmente non succede mai perché i vertici normali vengono ricalcolati se la trama non li ha. Potrebbe accadere a causa di un plug-in spazio tangente personalizzato difettoso. |
| Impossibile trovare tangenti di vertice nella trama [nome trama]. | Come sopra. |
| Impossibile trovare il binomio dei vertici nella trama [nome trama]. | Come sopra. |
| Impossibile trovare i colori dei vertici nella trama [nome trama]. | Nessun colore dei vertici trovato nella trama specificata. Questo può accadere se almeno una sottorete nella trama di poli superiore non ha alcun colore di vertice definito. |
| Dati insufficienti nel poly alto per utilizzare il fornaio selezionato. Interrompe il pane. | Preceduta da almeno uno dei messaggi precedenti. Normalmente, se nella scena mancano solo alcuni dati (ad esempio, una sola trama in una scena con poli elevato non presenta i colori dei vertici), il processo di cottura al forno riempie i dati mancanti con zeri e continua a cuocere. Se mancano troppi dati, questo messaggio viene inviato e il processo di cottura viene interrotto. |

## Texture trasferita dalla trama

| *Messaggio* | *Descrizione* |
| --- | --- |
| Caricamento della texture dei dettagli non riuscito. | Impossibile caricare la texture definita nelle impostazioni del fornaio. Il problema potrebbe essere dovuto al fatto che il file non è presente sul disco o è danneggiato e non leggibile. |
