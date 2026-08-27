---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: Usa le impostazioni dimensioni fisiche per ridimensionare i materiali Substance in base alle dimensioni reali in Unreal Engine 5.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Physical Size - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dimensioni fisiche - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Dimensioni fisiche - UE5

La dimensioni fisiche nei materiali di Substance consente di ridimensionare i materiali in base alle loro dimensioni nel mondo. Questo valore viene impostato in Substance Designer e letto in Irreale tramite il sistema di modelli di materiale.\
Il materiale [Substance\_Triplanar\_Template](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md) nella pagina principale contiene un esempio di come la dimensioni fisiche può essere utilizzata per ridimensionare i materiali irreali.



Indipendentemente dai valori di ingrandimento sulla trama, i materiali verranno affiancati in base alle dimensioni che occupano nel mondo in centimetri. Nel caso del materiale roccioso (figura 1), si tratta di 1,8 m (180 cm) per ciascuna misurazione.

![](../../../../assets/rock-material-parameters.png)

I valori dei materiali Substance contenenti dati dimensioni fisiche verranno copiati in qualsiasi nodo di parametro vettoriale del materiale esistente denominato dimensione fisica.



Poiché non è presente alcun valore di spostamento nei materiali in UE5, il modello di dimensioni fisiche copia il valore come X, Y, X per la mappa triplanare.
