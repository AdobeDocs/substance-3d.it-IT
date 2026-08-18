---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/physical-size-in-blender.html"
breadcrumb-title: ''
description: Usa le impostazioni dimensioni fisiche per ridimensionare i materiali Substance in base alle dimensioni reali in Blender.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Physical size in Blender
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dimensioni fisiche in Blender
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Dimensioni fisiche in Blender

La dimensioni fisiche nei materiali di Substance consente di ridimensionare i materiali in base alle loro dimensioni nel mondo. Le dimensioni sono impostate in applicazioni Substance come Designer e mostrate nella sezione Dimensioni fisiche del pannello dei plug-in.

![](../../../assets/blender-physical-size.png)

Con la Dimensioni fisiche abilitata, i materiali verranno affiancati in base alle loro dimensioni reali in centimetri. L&#39;affiancatura del materiale rimarrà la stessa indipendentemente dalla scala degli oggetti. La funzione può essere attivata passando allo shader di Dimensioni fisiche nel pannello del componente aggiuntivo. Dopo aver regolato la scala di un oggetto, la scala deve essere applicata con ctrl/comando+A per affiancare con precisione la texture della Dimensioni fisiche.

## Regolazione della Dimensioni fisiche

I valori nel nodo di mappatura possono essere regolati per il controllo artistico sulla suddivisione in porzioni delle Dimensioni fisiche. Inoltre, per controllare la mappatura della texture utilizzando le trasformazioni dell’oggetto di input, potete utilizzare un oggetto come un oggetto Vuoto per l’input Coordinate texture (vedete l’esempio seguente).

![](../../../assets/blender-physical-szie-empty.gif)
