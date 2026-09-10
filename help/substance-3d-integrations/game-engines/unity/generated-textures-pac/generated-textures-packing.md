---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/game-engines/unity/generated-textures-packing.html"
breadcrumb-title: ''
description: Scopri come Substance genera texture in Unity e configura l'impacchettamento texture per gli input di shader ottimali.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Generated Textures (Packing)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texture generate (Impacchettamento)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 6%

---


# Texture generate (Impacchettamento)

Le Texture generate mostrano gli output della Substance che vengono calcolati dalla Substance Engine per creare texture. Queste texture vengono inserite negli shader. Per impostazione predefinita, vengono creati solo gli input di base utilizzati dallo shader. Se l’opzione &quot;Genera tutti gli output&quot; è abilitata, tutte le texture verranno mostrate qui.

![](../../../assets/screen-shot-2022-03-29-at-1-24-16-pm-copy.png)

Quando l’opzione &quot;Genera tutti gli output&quot; è abilitata

![](../../../assets/screen-shot-2022-03-29-at-1-29-35-pm-copy.png)

## Utilizzo

1. Se si seleziona un&#39;icona texture, la texture viene selezionata nella finestra del progetto. Questo non funziona per i materiali di runtime perché le texture non vengono generate nella cartella del progetto.
1. Il pulsante sRGB funziona in modo simile all’opzione sRGB (texture colori) nelle Texture di importazione. Consente di impostare se una texture deve essere interpretata in uno spazio gamma (sRGB) o lineare. Il plug-in Substance gestisce automaticamente questa interpretazione, ma può essere sostituita se necessario.

   | Substance output | sRGB |
   | --- | --- |
   | Colore di base | Attivato |
   | Diffusione | Attivato |
   | Speculare | Attivato |
   | Normale | Disattivato |
   | Metallizzato | Disattivato |
   | Ruvidità | Disattivato |
   | Lucidità | Disattivato |
   | Altezza | Disattivato |
   | Occlusione ambientale | Disattivato |

## Canali di Impacchettamento

È possibile comprimere una texture nel canale alfa di un&#39;altra texture utilizzando il menu a discesa. Ogni texture generata dispone di un menu a discesa che contiene un elenco di tutti gli output della texture generati dai materiali della Substance. È sufficiente scegliere una mappa dall&#39;elenco per inserirla nel canale alfa della texture. L’opzione Sorgente corrisponde al canale alfa della texture.

In questa immagine, ho selezionato la mappa dell&#39;altezza:

![](../../../assets/screen-shot-2022-03-29-at-2-48-33-pm.png)

Nell&#39;immagine seguente, è possibile vedere che l&#39;output del height viene imballato nel canale alfa della mappa del colore di base.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-29-at-2-53-20-pm-copy?$png$&jpegSize=200&wid=1248)

## Mappatura Texture di output

Inoltre, la texture di output può essere assegnata individualmente agli Input di superficie dei materiali Unity tramite la sezione Mappatura Texture di output. Le texture di output generate dal file .sbsar verranno visualizzate nella colonna di sinistra, mentre gli Input superficie unità disponibili verranno visualizzati nella colonna di destra. Quest’ultimo può essere modificato mediante i menu a discesa.

![](../../../assets/image2023-3-27-14-30-24.png)
