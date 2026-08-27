---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-map-has-strange-colorful-gradients.html"
breadcrumb-title: ''
description: Correggi strane sfumature colorate nelle mappe normali controllando le normali della trama, i gruppi di arrotondamento e la mappatura UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal map has strange colorful gradients
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La mappa normale ha strane sfumature colorate
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# La mappa normale ha strane sfumature colorate

L&#39;output del fornaio è costituito da una serie di sfumature colorate molto forti.

![](../../assets/color-gradient.png)


## Descrizione

Le sfumature colorate di solito si verificano quando vi è una mancata corrispondenza tra la trama a poli alto e a poli basso durante il processo di cottura al forno. Questa mancata corrispondenza può essere spiegata con il seguente motivo:

* La trama <b>high-poly e low-poly non si sovrappone</b> correttamente (vedere l&#39;immagine seguente).
* Il poly alto è <b>geometria mancante</b> che il poly basso tenta di coprire.
* La trama ad alto poli o a basso poli ha invertito le normali dei vertici.

Quando accade, il processo di cottura tenta di far corrispondere una geometria che non esiste, creando qualcosa di vuoto. Il fornaio riempie quest&#39;area vuota con un colore estratto dai pixel adiacenti nelle texture che crea la sfumatura colorata (a meno che <b>Diffusione</b> non sia disattivato).

## Soluzione

Considerate le poche ragioni possibili che possono portare a una non sovrapposizione delle maglie, è necessario prendere in considerazione alcune soluzioni:

* Assicuratevi di congelare/reimpostare la trasformazione della trama (reimpostare la forma x, ecc.) per assicurarvi che tutte le trame siano coerenti
* Importa la trama bassa e alta come poly nel software di modellazione 3D per verificare che si sovrappongano correttamente
* Assicurati che la convenzione di denominazione sia valida se utilizzi la funzione [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md) (puoi verificarla effettuando una cottura in forno e quindi esaminando il file di registro che dovrebbe stampare i nomi delle trame).

### Esempio

Di seguito è riportato un esempio con una sfera ad alto e basso poli. A sinistra le trame non si sovrappongono perché il poligono superiore è stato allontanato:

![](../../assets/baking-gradients.jpg)
