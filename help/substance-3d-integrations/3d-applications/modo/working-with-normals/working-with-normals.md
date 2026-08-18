---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-normals.html"
breadcrumb-title: ''
description: Configura le impostazioni di orientamento delle mappe normali in MODO per garantire un rendering delle mappe normale corretto con i materiali delle Substance.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilizzo dei valori normali
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# Utilizzo dei valori normali

Utilizzo dei dati normali: impostazione dell&#39;orientamento corretto

Le Substance Stock sono create per utilizzare l&#39;orientamento normale DX. Tuttavia, MODO utilizza OGL. Potete capovolgere la normale impostando il parametro Formato normale su 1.0. Il plug-in Substance interpreterà solo i parametri impostati nella Substance. È possibile che una Substance non disponga del parametro &quot;normal\_format&quot; poiché spetta all&#39;autore della Substance aggiungere questo controllo alle Substance personalizzate. Se una Substance non presenta questo parametro, potete capovolgere il canale verde sul livello Texture della mappa normale per correggere l’orientamento.

>[!NOTE]
>
> L’inversione del canale verde avviene solo se la Substance ha un orientamento normale errato e l’autore non ha creato un controllo che consenta di invertire la normale nei parametri della Substance

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/normal-1.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/invert-2.png)

</td>
</tr>
</table>
