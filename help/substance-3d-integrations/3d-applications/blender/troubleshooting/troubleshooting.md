---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/blender/troubleshooting.html"
breadcrumb-title: ''
description: Diagnostica e risolvi i problemi più comuni con il componente aggiuntivo Substance 3D in Blender utilizzando la console di sistema.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Risoluzione dei problemi
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# Risoluzione dei problemi

La console di sistema può essere utilizzata per diagnosticare gli errori rilevati durante l&#39;utilizzo del componente aggiuntivo. La finestra della console di sistema di Blender viene aperta in modo diverso a seconda del sistema operativo. Per istruzioni dettagliate, segui i passaggi nella [pagina della documentazione](https://docs.blender.org/manual/en/2.79/advanced/command_line/introduction.html#console-window-status-and-error-messages) della console di sistema di Blender. L’output della console può essere utile quando si verificano problemi imprevisti, ad esempio quando le texture non vengono caricate o i materiali si bloccano nell’elaborazione.

Per segnalare un bug, partecipa al canale #substance-blender-beta sul [server Discord Substance](https://discord.com/invite/substance3d) o visita le [community di Adobe](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender). Le informazioni pertinenti dal registro della console e le eventuali fasi di riproduzione per il problema possono essere incluse nei report.

## Problemi comuni e soluzioni

* *Errori della console correlati a WMIC.*
  * *A volte le installazioni di Windows non includeranno WMIC, il che è necessario in questo caso. Di seguito viene illustrato come risolvere manualmente il problema:*
    * Seleziona Impostazioni - Sistema - Funzioni opzionali
    * Selezionare &quot;Visualizza funzionalità&quot;, quindi selezionare &quot;Aggiungi funzionalità&quot;
    * Viene visualizzata una nuova finestra, scorri l&#39;elenco verso il basso per trovare WMIC, seleziona la casella di controllo, quindi premi Avanti e nella finestra successiva premi Aggiungi.
    * Verrà visualizzata una nuova finestra che mostra l&#39;avanzamento dell&#39;installazione di WMIC in Azioni recenti.
    * *Il download potrebbe richiedere alcuni minuti. Dopo questo, reimposta il computer e riavvia Blender e il componente aggiuntivo. Quando si fa clic sul caricamento nel pannello Substance 3D, viene visualizzata la finestra dell&#39;elenco dei file.*
  * Se il problema persiste, potrebbe essere necessario definire WMIC nelle variabili PATH. Fare riferimento alla documentazione relativa alla versione specifica di Windows.
* *Non tutte le impostazioni vengono visualizzate nel pannello Substance 3D dopo l&#39;aggiornamento del componente aggiuntivo e il caricamento di un materiale.*
  * Ciò può verificarsi quando si rimuove una versione precedente del componente aggiuntivo e si installa una versione più recente nella stessa sessione, poiché i file più vecchi possono ancora essere memorizzati nella cache del sistema.\
    Il riavvio di Blender deve rendere effettive le modifiche.
* *Problemi durante l&#39;installazione del componente aggiuntivo./ I materiali sono bloccati nell&#39;elaborazione tra le sessioni. / I materiali non generano texture tra una sessione e l’altra. / Errori durante il caricamento dei file .sbsar.*
  * Questo potrebbe essere un problema con l’installazione degli strumenti di integrazione e generalmente viene risolto rimuovendo manualmente gli strumenti. Per istruzioni sulla rimozione manuale, visita la pagina [Disinstallazione del componente aggiuntivo](../../../3d-applications/blender/uninstalling-the-add-on/uninstalling-the-add-on.md).
* *I materiali non vengono aggiornati nella visualizzazione di rendering dei cicli*.
  * Per impostazione predefinita, il componente aggiuntivo non aggiorna le texture nella vista di rendering dei cicli. Tuttavia, possono essere aggiornati forzatamente attivando <b>Cicli Aggiornamento automatico texture</b>nelle preferenze del componente aggiuntivo.
* I parametri vengono ripristinati dopo il salvataggio nella visualizzazione di rendering dei cicli.
  * Si tratta di un problema noto relativo alla memorizzazione in cache sul lato Blender che è di sola lettura. Durante il salvataggio, non viene inviato alcun messaggio al motore remoto per aggiornare i file di texture generati. Le texture appariranno normali dopo aver lasciato la vista di rendering dei cicli e aver ripristinato la vista.
* *I materiali non vengono più aggiornati dopo aver annullato o modificato i parametri.*
  * I materiali potrebbero non essere aggiornati dopo aver annullato le azioni. Anche se i parametri torneranno allo stato precedente, le texture non verranno annullate per corrispondere. Per aggiornare nuovamente la texture, usate il pulsante Aggiorna per ripristinare i parametri predefiniti e ricaricare le texture.
* *I colori impostati nel Substance Designer vengono visualizzati in modo leggermente diverso nel selettore colore di Blender e i valori cromatici non sono gli stessi.*
  * Blender applica una correzione gamma solo ai colori del selettore Colore di Blender. Anche se questo causa una discrepanza nel selettore colore, i colori visualizzati nelle texture sono precisi rispetto ai valori impostati nelle app Substance.
* Errore della console *&quot;wmic non riconosciuto&quot; durante il caricamento di un materiale in Windows.*
  * Questo problema si verifica quando C:\Windows\System32\wbem\ non è incluso nelle variabili di sistema PATH. Fare riferimento alla documentazione relativa alla versione specifica di Windows.
* Errore *&quot;Tipo CPU non valido eseguibile&quot; in Mac.*
  * Questo problema si verifica quando Rosetta non è abilitato sui computer ARM Mac. Per ulteriori informazioni, vedere [Pagina Rosetta di Apple](https://support.apple.com/en-us/102527). Per ulteriori istruzioni, consulta inoltre questa [guida all&#39;installazione](https://medium.com/@jithmisha/fix-for-macbook-air-m1-m2-bad-cpu-type-in-executable-error-3719a0a1cb6).
* *Le modifiche apportate al grafico dello shader vengono annullate quando si utilizza il pulsante Aggiorna o si aggiornano i parametri.*
  * Il componente aggiuntivo ha aggiornato le connessioni nel grafico dopo modifiche o aggiornamenti. Per ovviare a questo problema, duplica il materiale di fusione creato dal file .sbsar e assegnagli un nuovo nome. Aggiungere i nodi solo al duplicato. Le texture verranno aggiornate nel gruppo di nodi mantenendo i nodi aggiunti dall&#39;utente. Durante l&#39;aggiornamento, copia questi nodi e incollali in un nuovo grafico dopo l&#39;aggiornamento.
