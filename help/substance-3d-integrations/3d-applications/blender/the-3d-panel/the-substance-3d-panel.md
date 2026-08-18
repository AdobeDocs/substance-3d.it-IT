---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/the-substance-3d-panel.html"
breadcrumb-title: ''
description: Scopri come utilizzare il pannello Substance 3D in Blender per gestire materiali, parametri e output.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > The Substance 3D Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Il pannello Substance 3D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# Il pannello Substance 3D

![](../../../assets/blender-substance3dpanel.png)

## Controlli del pannello

**Crea** - Apre l&#39;elenco dei file per selezionare un materiale Substance 3D. Per impostazione predefinita, viene creato un materiale di fusione utilizzando texture generate dal file .sbsar.

**Applica** - Collegate il materiale Substance 3D selezionato agli oggetti selezionati in un nuovo slot di materiale. Questa operazione non sostituisce le precedenti assegnazioni di materiale sull&#39;oggetto.

**Risorse community Substance 3D**: apre la pagina Risorse community Substance 3D nel browser Web.

**Substance 3D Assets**: apre la pagina di origine della Substance 3D Assets nel browser Web.

**Duplica materiale Substance 3D selezionato** - Carica una nuova istanza del materiale Substance 3D selezionato. I parametri delle diverse varianti dello stesso materiale di Substance possono essere regolati indipendentemente l&#39;una dall&#39;altra.

**Aggiorna** - Ricarica il materiale Substance 3D

>[!WARNING]
>
> **Avviso:**
> 
> Se si utilizza il pulsante Aggiorna, eventuali modifiche apportate dall’utente al grafico shader verranno annullate. Copia tutti i nodi aggiunti dall&#39;utente prima dell&#39;aggiornamento per incollarli nel grafico dopo l&#39;aggiornamento.

**Rimuovi**: rimuove il materiale Substance 3D selezionato dal pannello.

>[!NOTE]
>
> Il materiale di fusione creato dal materiale di Substance rimarrà nel progetto. Può essere eliminato o rimosso manualmente dagli oggetti.

**Materiali Substance 3D caricati** - Visualizza un elenco dei Materiali Substance caricati nel file .blend.

## Parametri grafico

**Risoluzione output** - Menu a discesa per la risoluzione con e height. Questi possono essere scollegati per regolare i valori in modo indipendente.

**Numero casuale e numero casuale**: il pulsante di generazione casuale genera un nuovo valore di numero casuale per modificare i parametri che possono utilizzare valori casuali. Il valore di inizializzazione casuale può essere impostato anche manualmente.

## Utilizzo dei predefiniti

I file SBSAR possono essere pubblicati con i predefiniti, che si trovano nella casella a discesa Predefiniti. Per creare predefiniti personalizzati, regolare i parametri nel modo desiderato e utilizzare il pulsante **Salva**. Sono disponibili ulteriori opzioni per esportare il predefinito selezionato come file .sbsprs e per eliminare il predefinito selezionato dall’elenco a discesa. Il pulsante **Carica** può essere utilizzato per importare i predefiniti dai file .sbsprs.

## Substance parametri

I parametri esposti in Substance Designer possono essere regolati mediante i controlli Substance parametro. Questi parametri sono impostati dal creatore del Materiale Substance e variano tra i materiali. La regolazione di questi parametri aggiornerà le texture generate, come indicato dall’icona di elaborazione accanto al nome del materiale nella sezione Materiali Substance 3D caricati.

Il formato di file delle texture di output può essere alternato e modificato tramite i menu a discesa.

Per ulteriori informazioni, vedere [Esposizione di un parametro](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter) nella pagina della documentazione di Designer.

## Parametri tecnici

I materiali di Substance possono avere una serie di parametri tecnici. Questi sono controlli aggiuntivi per la correzione del colore e altre regolazioni del materiale.
