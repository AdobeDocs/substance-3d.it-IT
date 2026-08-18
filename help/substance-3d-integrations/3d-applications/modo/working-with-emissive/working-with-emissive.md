---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-emissive.html"
breadcrumb-title: ''
description: Configurare le proprietà di emissione per i materiali Substance in MODO per controllare la quantità luminosa e le impostazioni del colore.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Emissive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo di Emissive
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Utilizzo di Emissive

## Utilizzo dell’effetto Emissivo (quantità e colore luminosi)

La Substance può avere un output di emissione opzionale. Potete usare questo metodo come Quantità luminosa e Colore in MODO. Quando attivi l’output di emissione, questo viene impostato sull’effetto Quantità luminosa. Per impostazione predefinita, questo canale viene interpretato come lineare nella scheda Texture immagine fissa.\
Fate clic con il pulsante destro del mouse sulla texture nell’albero Shader e scegliete Duplica. Quindi, impostate la texture emissiva duplicata sull’effetto Colore luminoso. Potete quindi apportare modifiche ai valori più alto e più basso per la texture che determina l’effetto Quantità luminosa per intensificare ulteriormente il valore.

>[!NOTE]
>
> Per la texture impostata su Colore luminoso, è necessario impostare l’interpretazione su sRGB nella scheda Immagine fissa.

Per ottenere un effetto fiorito, è necessario abilitare Bloom nel pannello Rendering e impostare Soglia e Raggio.

![](../../../assets/bloom.png)

Per i materiali Unreal e Unity, l&#39;output Emissivo è gestito in modo specifico dal materiale.\
Irreale = Irreale Emissivo\
Unità = Emissioni unitarie

Le texture Emissione irreale e Emissione unitaria devono essere modificate da Lineare a sRGB nella scheda Immagine fissa.
