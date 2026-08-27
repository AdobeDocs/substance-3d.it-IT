---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: Abilita il Raytracing GPU con accelerazione hardware per velocizzare i calcoli di baking di 25 volte o più, per flussi di lavoro più veloci.
helpx_creative_field: ""
helpx_description: bakers > Features > GPU Raytracing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Raytracing GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 18%

---


# Raytracing GPU

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Alcuni fornai supportano l&#39;accelerazione hardware del ray tracing sulla GPU, che di solito aumenta la velocità di calcolo di un fattore di 25 o superiore.

## Requisiti hardware

Il ray tracing verrà attivato automaticamente se il sistema soddisfa i seguenti requisiti:

* È installata una GPU compatibile\* (serie RTX, Titan V o GeForce 10xx)
* I driver della GPU sono aggiornati
* Windows 10 &quot;Autunno Creator&quot; / Aggiornamento di ottobre (versione 1809) o successiva è installato\*\*

</td>
<td style="border: 0;" valign="top">

![Confronto Raytracing GPU on/off](../../assets/rtx-ao-demo.gif "Confronto Raytracing GPU on/off"){zoomable="yes"}

</td>
</tr>
</table>

\*: le GPU NVIDIA compatibili includono tutte le GPU che utilizzano l&#39;architettura Pascal o versioni più recenti. Ad esempio, le serie GTX 10, Titan V, RTX 20 o più recenti.

\*\*: per verificare la versione di Windows in uso, scegliere &#39;winver&#39; dal menu Start e premere Invio.\
L&#39;aggiornamento è disponibile nella [pagina dedicata](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update) del sito Web del supporto tecnico Microsoft.

>[!TIP]
>
> In caso di problemi, Raytracing GPU può essere disattivato nelle preferenze dell’applicazione.

## Panettieri supportati

Le tabelle seguenti elencano il supporto Raytracing GPU per ogni panettiera, in base alla versione dei panettieri Substance 3D:

+++Versione 3 e successive

| Baker | Supporta Raytracing GPU |
| --- | --- |
| Occlusione ambientale | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Normale con curvatura | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Colora | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Curvatura | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Altezza | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Normale | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Spazio mondo normale | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |



| Baker | Supporta Raytracing GPU |
| --- | --- |
| Maschera di opacità | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Posizione | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Posizione bassa | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Spessore | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Texture trasferita | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Da mondo a tangente | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


+++

+++Versione 2

| Baker | Supporta Raytracing GPU |
| --- | --- |
| Occlusione ambientale | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Occlusione ambientale da trama | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Mappa normale da trama | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Colore da trama | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Converti UV in SVG | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Curvatura da trama | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Altezza da trama | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Normale da trama | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |



| Baker | Supporta Raytracing GPU |
| --- | --- |
| Maschera di opacità dalla trama | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Posizione da trama | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Posizione | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Spessore da trama | <div><img alt="(spuntare)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Texture trasferita da trama | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Direzione dello spazio mondiale | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Normali spaziali mondiali | <div><img alt="(errore)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


\*: supporta il raytracing CPU, che è notevolmente più lento del Raytracing GPU.

+++
