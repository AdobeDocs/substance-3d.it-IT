---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/home.html"
breadcrumb-title: ''
description: Scoprite come utilizzare Substance Baker per calcolare le informazioni basate sulle trame nei file di texture e migliorare il flusso di lavoro per la creazione di texture.
helpx_creative_field: ""
helpx_description: bakers > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance Bakers
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 13%

---


# Substance Bakers

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

<b>Substance Bakers</b> è un set di strumenti avanzati per il calcolo di informazioni basate su mesh nei file texture. Possono essere utilizzati da qualsiasi artista con una trama 3D per sfruttare i metodi di texture avanzati. La esegue i baking è un processo fondamentale del flusso di lavoro del software Substance per offrire<b> potenti strumenti</b> e <b>creazione automatizzata delle texture</b>.

Questa documentazione descrive le <b>nozioni fondamentali per eseguire i baking</b> e i <b>problemi comuni</b> e gli errori che possono verificarsi durante l&#39;esecuzione di questa procedura.

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](../assets/optim-baker-home.png){width="400px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## Introduzione

* [Che cosa si Esegue i baking?](../getting-started/what-is-baking/what-is-baking.md)
* Esegue i baking con:
  * [Substance 3D Painter](../getting-started/software-interface/3d-painter/substance-3d-painter.md)
  * [Substance 3D Designer](../getting-started/software-interface/3d-designer/substance-3d-designer.md)
  * [Substance 3D Automation Toolkit](../getting-started/software-interface/3d-automation-toolkit/substance-3d-automation-toolkit.md)
* [Disponibilità per software](../getting-started/availability-per-software/availability-per-software.md)
* [Software 3D compatibile](../getting-started/compatible-3d-software/compatible-3d-software.md)
* [Tutorial](../getting-started/tutorials/tutorials.md)

</td>
<td style="border: 0;" valign="top">

### Impostazioni forni

* [Parametri comuni](../bakers-settings/common-parameters/common-parameters.md)
* [Occlusione ambientale](../bakers-settings/ambient-occlusion/ambient-occlusion.md)
* [Occlusione ambientale dalla trama](../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)
* [Normali incurvate da trama](../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)
* [Mappa colori da trama](../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)
* [Converti UV in SVG](../bakers-settings/convert-uv-to-svg/convert-uv-to-svg.md)
* [Curvatura](../bakers-settings/curvature/curvature.md)
* [Curvatura da trama](../bakers-settings/curvature-from-mesh/curvature-from-mesh.md)
* [Curvatura da trama (obsoleta)](../bakers-settings/curvature-from-mesh-dep/curvature-from-mesh-deprecated.md)
* [Mappa altezza dalla trama](../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)
* [Mappa normali da trama](../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)
* [Maschera di opacità da trama](../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)
* [Posizione](../bakers-settings/position/position.md)
* [Mappa posizione da trama](../bakers-settings/position-map-from-mesh/position-map-from-mesh.md)
* [Mappa spessore da trama](../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)
* [Texture trasferita da trama](../bakers-settings/transferred-texture-from/transferred-texture-from-mesh.md)
* [Direzione spazio globale](../bakers-settings/world-space-direction/world-space-direction.md)
* [Normali spazio globale](../bakers-settings/world-space-normals/world-space-normals.md)

</td>
<td style="border: 0;" valign="top">

### Guide

* [Messaggi di errore e di avvertenza](../guides/error-and-warning-mes/error-and-warning-messages.md)
* [Prestazioni e ottimizzazione](../guides/performances-and-opt/performances-and-optimizations.md)
* [Triangolazione prima della cottura](../guides/triangulating-before-bak/triangulating-before-baking.md)

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Funzioni

* [Cache geometria](../features/geometry-cache/geometry-cache.md)
* [Raytracing GPU](../features/gpu-raytracing/gpu-raytracing.md)
* [Corrispondenza per nome](../features/matching-by-name/matching-by-name.md)
* [Spazio tangente](../features/tangent-space/tangent-space.md)

</td>
<td style="border: 0;" valign="top">

### Domande frequenti

* [Come si esportano le mappe con baking?](../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)
* [Il dithering viene applicato alle texture cotte?](../common-questions/dithering-applied-baked/is-dithering-applied-to-baked-textures.md)
* [È necessario abilitare &quot;Calcola spazio tangente per frammento&quot;?](../common-questions/should-enable-compute-tan/should-i-enable-compute-tangent-space-per-fragment.md)
* [Texture eseguita i baking all&#39;esterno del software Substance non sembra corretta](../common-questions/texture-baked-outside-sof/texture-baked-outside-of-substance-software-looks-incorrect.md)
* [Che cosa sono i file Assbin?](../common-questions/what-are-assbin-files/what-are-assbin-files.md)
* [Qual è la profondità di bit delle texture eseguite i baking?](../common-questions/what-the-bit-depth-baked/what-is-the-bit-depth-of-baked-textures.md)
* [Qual è la differenza tra OpenGL e il formato normale DirectX?](../common-questions/what-the-difference-bet/what-is-the-difference-between-the-opengl-and-directx-normal-format.md)
* [Perché ci sono allungamento strani nelle mie texture dopo aver eseguito i baking o esportato?](../common-questions/why-are-there-strange-str/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.md)
* [Perché la funzione Corrispondenza per nome non funziona con Occlusione/Thickness ambiente?](../common-questions/why-matching-name-not-wor/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.md)
* [Perché la mia maglia è completamente nera dopo aver eseguito i baking?](../common-questions/why-mesh-fully-black-aft/why-is-my-mesh-fully-black-after-baking.md)

</td>
<td style="border: 0;" valign="top">

### Problemi comuni

* [Alias sulle giunture UV](../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)
* [L&#39;output del baker è completamente nero o vuoto](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/baker-output-is-fully-black-159451835.html)
* [Esegue i baking non riuscita con Mappe colori da mesh](../common-issues/baking-failed-with-color/baking-failed-with-color-map-from-mesh.md)
* [Sulla superficie della trama è visibile una croce di ombreggiatura nera](../common-issues/black-shading-cross-are/black-shading-cross-are-visible-on-the-mesh-surface.md)
* [Le parti della trama sanguinano tra loro](../common-issues/mesh-parts-bleed-between/mesh-parts-bleed-between-each-other.md)
* [La mappa normale ha strane sfumature colorate](../common-issues/normal-map-has-strange/normal-map-has-strange-colorful-gradients.md)
* [Texture normale con aspetto sfaccettato](../common-issues/normal-texture-looks-fac/normal-texture-looks-faceted.md)
* [Le giunture sono visibili dopo aver eseguito i baking una texture normale](../common-issues/seams-are-visible-after/seams-are-visible-after-baking-a-normal-texture.md)
* [Cucitura visibile su ogni volto](../common-issues/seam-visible-every-face/seam-visible-on-every-face.md)

</td>
</tr>
</table>
