---
helpx_url: "https://helpx.adobe.com/it/substance-3d-general/ecosystem/substance-for-linux.html"
breadcrumb-title: ''
description: Scopri come scaricare, installare e attivare le applicazioni Substance 3D su Linux utilizzando il portale Adobe Download Access.
helpx_creative_field: ""
helpx_description: Substance 3D General
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D per Linux (ADA)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 081136918fdf7f431ecee47e5ce64d8b5235bb1b
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# Guida alla distribuzione

Dopo aver acquistato Substance 3D per Linux® tramite il contratto Enterprise, i prodotti e le licenze corrispondenti vengono forniti sul portale [Adobe Download Access (ADA)](https://download-access.adobe.com/lws/downloads). Per distribuire correttamente il software, dovrai scaricare sia le build del software che i file delle chiavi di licenza da ADA.

## Scarica le build software e i file delle chiavi di licenza:

Accedi a [Accesso download Adobe](https://download-access.adobe.com/lws/downloads). Trova le build software e i file delle chiavi di licenza:

1. Utilizzare il menu a discesa Account per selezionare l&#39;account su cui è stato acquistato Substance 3D Linux.

   ![](../../assets/ADA1.png)
1. Seleziona Download con il collegamento nell’intestazione della pagina.

   ![](../../assets/ADA2.png)
1. Fai clic su Visualizza download nel prodotto corrispondente.

   ![](../../assets/ADA3.png)
1. ADA caricherà le informazioni sulla licenza associate a questo ID e le visualizzerà nella tabella seguente.
1. Fare clic su &quot;Scarica&quot; nella riga &quot;Certificato digitale&quot; per scaricare il file zip contenente i file delle chiavi di licenza.

   * Il file zip contiene un codice di licenza per prodotto.
   * Il codice di licenza attiverà il prodotto su ciascuno dei computer con licenza.

   ![](../../assets/ADA4.png)
1. Fare clic su &quot;Substance 3D&quot; Sampler, Painter o Designer per visualizzare le versioni software di Substance 3D Painter, Substance 3D Designer e Substance 3D Sampler.
1. Fare clic su &quot;Scarica&quot; per scaricare il file di installazione del prodotto che si desidera installare.

   ![](../../assets/ADA5.png)
1. Viene visualizzata una notifica &quot;Download del software&quot;. Fai clic su &quot;Accetta&quot;.

   ![](../../assets/ADA6.png)

## Installazione e attivazione

Per installare il software:

1. Fai doppio clic sul file EXE del prodotto per avviare l&#39;installazione guidata.
1. Segui i passaggi per completare l’installazione.

Sono disponibili due opzioni per l&#39;attivazione del software: attivazione locale o attivazione di rete.

### Attivazione locale

1. Decomprimi la cartella zip scaricata da ADA.
1. Avvia il software da attivare.
1. Nella procedura guidata di attivazione, selezionare &quot;Attiva utilizzando un file di codice di licenza&quot;.

   ![](../../assets/LinuxActivation3.png)
1. Fare clic su &quot;Sfoglia&quot; e selezionare il percorso del file del codice di licenza corrispondente.
1. Fare clic su &quot;Avanti&quot; per attivare il software.

### Attivazione di rete

1. Decomprimi la cartella zip scaricata da ADA.
1. Inserire i file delle chiavi di licenza decompressi in una rete montata condivisa.
1. Nel computer dell&#39;utente, imposta una variabile di ambiente che punti al file del codice di licenza come spiegato in queste pagine:

   * Substance 3D Painter - <https://experienceleague.adobe.com/it/docs/substance-3d-painter/using/pipeline-and-integration/configuration/environment-variables>
   * Substance 3D Designer - <https://experienceleague.adobe.com/it/docs/substance-3d-designer/using/pipeline-and-project-configuration/environment-variables>
   * Substance 3D Sampler - <https://experienceleague.adobe.com/it/docs/substance-3d-sampler/using/pipeline-and-integrations/environment-variables>
