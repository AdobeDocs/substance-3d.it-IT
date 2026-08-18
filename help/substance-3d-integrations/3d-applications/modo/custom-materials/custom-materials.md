---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/custom-materials.html"
breadcrumb-title: ''
description: Utilizza i materiali personalizzati Unreal, Unity e glTF in MODO con il plug-in Substance per flussi di lavoro specializzati.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Custom Materials
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materiali personalizzati
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---


# Materiali personalizzati

Il plug-in Substance supporta i materiali personalizzati Unreal, Unity e glTF. Prima di caricare un file sbsar, è possibile selezionare la modalità di ombreggiatura che si desidera utilizzare.

## Sommario

## Materiale unità

Quando si utilizza l&#39;Unity Material (Materiale unitario), l&#39;effetto del livello del materiale viene impostato automaticamente. Il plug-in Substance posizionerà il materiale dell&#39;unità direttamente sopra il materiale dell&#39;articolo della Substance.

| Substance output | Spazio colore | Effetto livello materiale |
| --- | --- | --- |
| Colore di base | sRGB | Albedo unità |
| Lucidità | Lineare | Smoothness unità |
| Metallizzato | Lineare | Unity Metallic |
| Normale | Lineare | Unità normale |
| Con emissioni | sRGB | Emissione unità **\*impostata su sRGB sull&#39;immagine fissa** |
| Altezza | Lineare | Rilievo unità |
| Occlusione ambientale | Lineare | Occlusione ambiente unità |

![](../../../assets/unity-1.png){width="600px"}

## Materiale irreale

Quando si utilizza Materiale irreale, l’Effetto livello materiale viene impostato automaticamente. Il plug-in Substance posizionerà il materiale irreale direttamente sopra il materiale dell&#39;articolo della Substance.

| Substance output | Spazio colore | Effetto livello materiale |
| --- | --- | --- |
| Colore di base | sRGB | Colore di base irreale |
| Ruvidità | Lineare | Rugosità irreale |
| Metallizzato | Lineare | Metallico irreale |
| Normale | Lineare | Normale irreale |
| Altezza | Lineare | Rilievo irreale |
| Con emissioni | sRGB | Emissivo irreale **\*impostato su sRGB su immagine fissa** |
| Occlusione ambientale | Lineare | Occlusione ambientale irreale |
| Opacità | Lineare | Opacità irreale **\*deve deselezionare invertita sul livello texture** |

![](https://helpx-prod.scene7.com/is/image/HelpxProd/unreal?$png$&jpegSize=200&wid=1343){width="600px"}

Potrebbe essere necessario invertire il valore normale. Potete eseguire questa operazione dal menu Interpolazioni se la Substance dispone di un controllo per l’orientamento normale. In caso contrario, questa operazione può essere eseguita sulla texture stessa. Per ulteriori informazioni, vedere la pagina &quot;**[Utilizzo dei normali](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&quot;.

## materiale glTF

Quando si utilizza il materiale glTF, l&#39;effetto del livello di materiale verrà impostato automaticamente. Il plug-in Substance posizionerà il materiale glTF direttamente sopra il materiale dell&#39;elemento della Substance.

| Substance output | Spazio colore | Effetto livello materiale |
| --- | --- | --- |
| Colore di base | sRGB | Colore di base glTF |
| Ruvidità | Lineare | Rugosità glTF |
| Metallizzato | Lineare | glTF Metallic |
| Normale | Lineare | glTF Normale |
| Con emissioni | sRGB | glTF Emissiva **\*impostata su sRGB sull&#39;immagine fissa** |
| Occlusione ambientale | Lineare | occlusione ambiente glTF |

![](../../../assets/gltf.png){width="600px"}

Potrebbe essere necessario invertire il valore normale. Potete eseguire questa operazione dal menu Interpolazioni se la Substance dispone di un controllo per l’orientamento normale. In caso contrario, questa operazione può essere eseguita sulla texture stessa. Per ulteriori informazioni, vedere la pagina &quot;**[Utilizzo dei normali](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&quot;.
