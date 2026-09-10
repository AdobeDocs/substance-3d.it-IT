---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: Risolvi i problemi relativi al nero o al nero degli output di baker e scopri come risolvere i problemi relativi a trama e UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: L'output del baker è completamente nero o vuoto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# L&#39;output del baker è completamente nero o vuoto

>[!WARNING]
>
> **Problema**
> 
> Il risultato di un baker è una texture vuota o nera:
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **Spiegazione**
> 
> Una texture nera indica che il baker non è stato in grado di trovare le informazioni necessarie per generare un risultato. Ad esempio, durante la esegue i baking non è stata trovata la trama high-poly corrispondente a quella low-poly, con conseguente assenza di elementi da confrontare.

>[!NOTE]
>
> **Soluzione**
> 
> * Verificare che la trama high-poly necessaria per il baker sia stata caricata correttamente (per eventuali errori, fare riferimento al file di registro o alla finestra).
> * Verificare che le maglie a basso o alto poli non siano troppo grandi (più di un chilometro) o troppo piccole (meno di un centimetro).
> * Verificare se il baker è stato in grado di leggere/elaborare la trama (fare riferimento al file di registro/alla finestra per eventuali errori).
> * Verificare se la caratteristica [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md) non è stata configurata correttamente. Alcuni oggetti potrebbero escludersi a vicenda e non sovrapporsi mai.
> * Verificare che gli UV low-poly siano compresi nell&#39;intervallo 0-1.
