---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/color-management/substance-textures-in-maya.html"
breadcrumb-title: ''
description: Configura le impostazioni dello spazio colore per la texture Substance in Maya per garantire una gestione accurata del colore e il rendering.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management > Substance textures in Maya
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance texture a Maya
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# Substance texture a Maya

Lo spazio colore impostato per le mappe dipende dalle impostazioni e dalle regole definite nelle [Impostazioni di gestione colore Maya](https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-B260195C-A0FE-4F51-9EA2-099B61B7725A).

La Substance nel plug-in Maya è impostata su &quot;Ignora regole file spazio colore&quot; nel nodo file. Il plug-in si occupa dell&#39;impostazione dello spazio colore indipendentemente dalla Gestione colore, utilizzando quanto segue:

BaseColor, Diffusa, Emissivo, Specular = sRGB\
Normale, height, spostamento, rugosità, metallico = RAW

In genere, è necessario impostare lo spazio colore su RAW per le immagini che rappresentano dati non a colori. Tuttavia, questa impostazione può essere influenzata dalle regole impostate in Gestione colore.

![](../../../assets/raw.png)
