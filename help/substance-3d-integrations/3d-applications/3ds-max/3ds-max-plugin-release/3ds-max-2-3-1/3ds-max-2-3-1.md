---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-1.html"
breadcrumb-title: ''
description: Rivedi le note sulla versione per il plug-in 3ds Max versione 2.3.1 per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 3ds Max 2.3.1

Rilasciato il 13 febbraio 2020

Il plug-in ora viene installato all&#39;esterno della directory 3ds Max in C:\ProgramData\Autodesk\ApplicationPlugins\SubstanceIn3dsMax. Ora dovrebbe funzionare ovunque 3ds Max è detto di cercare i plug-in, quindi dovrebbe funzionare installato su un&#39;unità di rete, ecc.\
Si noti che il passaggio al plug-in applicazione e la directory di installazione cambiano lo rendono in modo che un aggiornamento da versioni 2.1.1 e precedenti non funzionerà correttamente. Questi dovrebbero essere rimossi manualmente per 3ds Max 2018 e 2019. La versione 2.2.0 deve essere aggiornata correttamente.\
Per alcuni dei problemi non risolti in questa versione, ne è prevista un’altra a breve per risolvere questi ed eventuali altri problemi.

Questa versione è attualmente disponibile per 3ds Max 2018, 2019, 2020 e 2021.

* Carica file .bsar ora cerca prima nella cartella delle immagini del progetto
* La finestra di dialogo di compatibilità del modulo di rendering viene visualizzata solo per il modulo di rendering per file VRay RT e VUE
* Trascinamento della selezione per l&#39;Editor materiale di ardesia disattivato per rimuovere i problemi con il batch Max
* La finestra di dialogo di rendering non viene più visualizzata nella modalità invisibile di Max 3ds
* Script python più piccoli ora compatibili con Python 3
* È stato aggiunto il supporto per l’utilità di avvio Substance per inviare le risorse Substance Source a 3ds Max. Ciò richiederà modifiche nel modulo di avvio, ma il supporto nel plug-in sarà disponibile quando la funzione verrà aggiunta.
* Lo script di rendering Redshift ora utilizza i nuovi nomi di nodi impostati in Redshift 2.6.24
* Massimo non più arresti anomali quando un percorso vuoto viene assegnato a Substance2 SubstanceFilePath
* Rimuovere la collisione del nome del tipo SubstanceOutput con il vecchio plug-in
* Classe SubstanceOutput rinominata in Substance2Output
* Classe rinominata Substance Menu Manager in Substance2MenuManager
* Gli ID blocco param vengono ora cancellati con forza quando si apre una scena, rimuovendo le collisioni tra i file di scena. Questo dovrebbe risolvere i problemi con blocchi di parametri non validi durante il caricamento quando si alternano le scene. L&#39;importazione può ancora comportare problemi, in quanto richiede modifiche più complesse
* Il plug-in è ora installato all&#39;esterno di 3ds Max. Tutti i percorsi sono stati modificati in relativi rispetto al percorso di caricamento.
* Il plug-in ora utilizza il sistema di plug-in Applicazione Autodesk.
