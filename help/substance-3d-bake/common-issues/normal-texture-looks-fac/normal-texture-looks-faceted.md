---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: Correggi l’aspetto sfaccettato nelle texture normali smussando le normali trame e regolando le impostazioni dei gruppi di arrotondamento.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texture normale con aspetto sfaccettato
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Texture normale con aspetto sfaccettato

>[!WARNING]
>
> **Problema**
> 
> La texture Normale appare sfaccettata o ogni faccia della trama è visibile in essa dopo averla eseguita i baking.
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **Spiegazione**
> 
> La ragione principale per cui eseguire i baking una normale produrrebbe questo risultato è perché le normali a bassa mesh poly non sono impostate correttamente. Ogni bordo di ogni faccia è un bordo duro, facendo in modo che la proiezione di raggi durante la corrispondenza con la trama ad alto poli ignori le informazioni vicine e crei cuciture o informazioni inconsapevoli. Anche se il risultato può sembrare a posto sulla trama, questo può portare a problemi di ombreggiatura in un secondo momento e deve essere risolto.

>[!NOTE]
>
> **Soluzione**
> 
> La soluzione principale è quella di rielaborare il vertice normale o la trama poly bassa, la denominazione esatta del processo dipende dal software di modellazione 3D:
> 
> * Usa **valori normali medi** a Maya, Houdini.
> * Utilizza **un gruppo di arrotondamento** in 3DS Max.
> * Usa **tonalità omogenea** in Blender.
> * Le trame esportate da zBrush saranno sempre sfaccettate e devono essere pulite in un altro software.
> 
> Tenete presente che questa operazione potrebbe non essere sufficiente: quando esportate una trama, assicuratevi che le impostazioni salvino/generino anche le informazioni relative alla normale del vertice o all’ombreggiatura.
