---
helpx_url: 'https://helpx.adobe.com/it/substance-3d-bake/features/matching-by-name.html'
breadcrumb-title: ''
description: Utilizzate la funzione Corrispondenza per nome (Matching by Name) per isolare le trame a basso e alto poli e impedire il sanguinamento della geometria durante la cottura al forno.
helpx_creative_field: ''
helpx_description: bakers > Features > Matching by Name
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Corrispondenza per nome
user-guide-description: ''
user-guide-title: ''
source-git-commit: d57629bee333101dd9f40f30ed24ff84b6b8c6f1
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---


# Corrispondenza per nome

![](../../assets/banner-matching-by-name.jpg)

Corrispondenza per nome è il nome di un metodo di filtraggio che può essere utilizzato in Substance Bakers per isolare le trame poly basse e poly alte in base al loro nome.

Questa funzionalità è molto utile per evitare che la geometria si dissolva l&#39;una sull&#39;altra durante il processo di cottura al forno per ottenere texture pulite. Per ottenere lo stesso risultato, evita di dover allontanare le trame (spesso definite &quot;esplose&quot;).

## Quando utilizzare Corrispondenza per nome

### Normale cottura mappa con sanguinamento mesh

In questo esempio il casco sopra la testa del personaggio sanguina sul volto del personaggio.

Abilitando Corrispondenza per nome possiamo ignorare il casco e cuocere correttamente il volto. *Questo risultato si basa sull&#39;impostazione Corrispondenza principale.*

| *Trama* | *Corrispondenza per nome disattivata* | *Corrispondenza Per Nome Su* |
| --- | --- | --- |
| ![](../../assets/baking-demo-vela.png){width="250px"} | ![](../../assets/baking-demo-vela-normal-nomatch.png){width="250px"} | ![](../../assets/baking-demo-vela-normal-withmatch.png){width="250px"} |

### Ignora backface per geometria mobile

In questo esempio, i &quot;pulsanti&quot; nella parte superiore della casella sono geometrie mobili, non sono collegati alla trama poly alta. Di conseguenza, per impostazione predefinita, le ombre verranno proiettate sulla casella sottostante, che mostrerà il bordo della geometria.

Abilitando l&#39;opzione Corrispondenza per nome per l&#39;impostazione **Ignora backface** possiamo eseguire l&#39;occlusione ambiente ignorando l&#39;area sotto i pulsanti per farla sembrare una singola casella.*Questo risultato si basa sull&#39;utilizzo dell&#39;impostazione Ignora sfondo.*

| *Trama* | *Corrispondenza per nome disattivata* | *Corrispondenza Per Nome Su* |
| --- | --- | --- |
| ![](../../assets/ignorebf-mesh.png){width="250px"} | ![](../../assets/ignorebf-off.png){width="250px"} | ![](../../assets/ignorebf-on.png){width="250px"} |

## Funzionamento della corrispondenza per nome

Il sistema Corrispondenza per nome funziona leggendo il nome della geometria nelle trame poly bassa e alta e utilizzando una parola chiave (il suffisso) per identificare/abbinare i nomi. Per impostazione predefinita i panettieri usano il suffisso specifico, ma possono cambiare (vedi di seguito).

I suffissi attualmente supportati sono:

| *Tipo di suffisso* | *Valore predefinito* | *Utilizzo* |
| --- | --- | --- |
| High Poly | *\_high* | Utilizzato per isolare il nome della trama poly alta in modo che corrisponda a quella poly bassa. |
| Low Poly | *\_low* | Utilizzato per isolare il nome della trama poly bassa in modo che corrisponda a quella poly alta. |
| Ignora faccia posteriore | *\_ignorebf* | Utilizzato per ignorare i caratteri di sfondo dei panettieri che utilizzano raggi secondari, ad esempio l&#39;Occlusione Ambiente.*Questo suffisso deve essere presente solo nelle trame di poli superiori, ad esempio:**mesh\_high\_ignorebf*** |

Alcune regole da prendere in considerazione per far funzionare correttamente questa funzione:

* La corrispondenza per nome deve essere abilitata in [Parametri comuni](../../bakers-settings/common-parameters/common-parameters.md) poiché è **disattivata per impostazione predefinita**.
* È possibile che in alcuni forni (ad esempio [Occlusione ambiente](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)) sia abilitata un&#39;impostazione secondaria Corrispondenza per nome, in quanto producono raggi secondari.
* La corrispondenza fa distinzione tra maiuscole e minuscole. Ciò significa che una trama denominata &quot;**Vela**&quot; non corrisponderà a un&#39;altra denominata &quot;**vela**&quot;.
* È possibile abbinare più trame in base alla posizione del suffisso nel nome della geometria.

Di seguito sono riportati alcuni esempi di come potrebbe funzionare la corrispondenza (utilizzando il suffisso predefinito):

| Nome poly basso | Corrispondenza con High Poly | Non Corrisponde A Poly Elevato |
| --- | --- | --- |
| <ul data-preserve-html="true"><li data-preserve-html="true">body_low</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">body_high</li><li data-preserve-html="true">body_high_top</li><li data-preserve-html="true">body_high_1</li><li data-preserve-html="true">body_high_2</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">body-high</li><li data-preserve-html="true">body_top_high</li></ul> |
| <ul data-preserve-html="true"><li data-preserve-html="true">Head_low</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Testa_alta</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">head_high</li></ul> |
| <ul data-preserve-html="true"><li data-preserve-html="true">Leg_low_top</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Gamba_alta</li><li data-preserve-html="true">Leg_high_top</li><li data-preserve-html="true">Leg_high_high_top</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Leg_top_high</li></ul> |

## Come impostare i panettieri

### Abilitazione della corrispondenza per nome

La corrispondenza per nome può essere abilitata in [Parametri comuni](../../bakers-settings/common-parameters/common-parameters.md) delle impostazioni di Baker:

| *Software* | *Impostazione della configurazione* |
| --- | --- |
| **Substance Painter** | <ol class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">     Aprite la finestra di cottura al forno (mediante le impostazioni del set di texture).    </li> <li class="step" data-preserve-html="true">     Visualizzare i parametri comuni.    </li> <li class="step" data-preserve-html="true">     Modifica l&#39;impostazione <strong>Corrispondenza</strong> da &quot;Sempre&quot; a &quot;Per nome trama&quot;.<br/> <img data-preserve-html="true" src="../../assets/baking-match-setting-sp.png"/>    </li> </ol> |
| **Substance Designer** | <ol class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">     Aprite la finestra Baking (facendo clic con il pulsante destro del mouse su una trama collegata nella finestra Esplora risorse).    </li> <li class="step" data-preserve-html="true">     Modificare l&#39;impostazione <strong>Corrispondenza</strong> da &quot;Sempre&quot; a &quot;Per nome trama&quot;. <br/> <br/>    </li> </ol> |

### Modifica dei nomi dei suffissi

I suffissi predefiniti sono \_low e \_high e possono essere modificati nel modo seguente:

* **Substance Painter**: nella [finestra di cottura](../../getting-started/software-interface/3d-painter/substance-3d-painter.md), entro i parametri comuni.
* **Substance Designer**: nelle [impostazioni del progetto](https://experienceleague.adobe.com/it/docs/substance-3d-designer/using/workspace/preferences/project-settings), sotto le impostazioni del forno.

## Trame ad alto poli da zBrush

Le trame a poli alti esportate da zBrush possono essere utilizzate per la cottura al forno con la funzione Corrispondenza per nome, tuttavia è possibile seguire alcune impostazioni:

| *Formato file* | *Descrizione* |
| --- | --- |
| **FBX** | Nessun parametro specifico da abilitare/disabilitare, i file mesh possono essere utilizzati così come sono. |
| **OBJ** | Per impostazione predefinita, i file OBJ esportati da zBrush non funzionano con **Nome corrispondente**. Invece, è possibile dire a Substance Painter di utilizzare il nome del file della trama per far corrispondere le trame per nome.Per farlo, assicurati di:<ol data-preserve-html="true"><li data-preserve-html="true"><strong>Disabilita</strong> il parametro Group (Grp) per <strong>ogni </strong> sottostrumento.</li><li data-preserve-html="true"><strong>Assegnare un nome</strong> appropriato al file OBJ (ad esempio: <strong>body_high.obj</strong>).</li></ol> ![](../../assets/zbrush-setting.png) |
