---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/renderers/color-management.html"
breadcrumb-title: ''
description: Comprendere la gestione del colore e la correzione gamma quando si utilizzano materiali Substance con diversi moduli di rendering.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestione colore
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 2%

---


# Gestione colore

L’approccio sarà semplice: il rendering dello spazio lineare fornisce la matematica corretta per i calcoli dell’illuminazione. Crea un ambiente che permette alle interazioni di luce di essere rappresentate in modo credibile nel mondo reale. Per una discussione sul rendering dello spazio lineare, dobbiamo introdurre il concetto di correzione gamma. Quando si codificano immagini per la visualizzazione e la memorizzazione, la correzione gamma rappresenta il processo di ottimizzazione per la riduzione della larghezza di banda e dell&#39;allocazione dei bit. Questo processo sfrutta la percezione della luminosità da parte dell’occhio umano, che segue approssimativamente la radice cubica della luminanza.

>[!NOTE]
>
> Il rendering dello spazio lineare è un soggetto molto complesso. Per ulteriori informazioni, consulta la [GUIDA PBR VOLUME ONE](https://academy.substance3d.com/courses/the-pbr-guide-part-1) gratuita su [Accademia Substance](https://academy.substance3d.com/).

## Gestione colore

Lo scopo di questo documento è quello di descrivere in dettaglio la procedura di utilizzo della texture esportata da **Substance Painter** e **Substance Designer** in [software 3D](https://www.adobe.com/it/products/substance3d/3d-augmented-reality.html) e moduli di rendering.

Il modo corretto di interpretare un’immagine utilizzata come input in un canale di materiale dipende da come l’immagine viene utilizzata nella scena. Anche lo spazio colore, la codifica e se i valori cromatici sono proporzionali alla **luminanza riferita alla scena** o alla **luminanza riferita alla visualizzazione** svolgono un ruolo importante.

* Le immagini utilizzate per rappresentare **dati non a colori** non devono essere Trasforma. Si tratta in genere di mappe **normali**, **rugosità**, **metalliche**, **spostamenti** e **ambientali** **occlusioni**.
* Le immagini che rappresentano i colori possono avere più scenari. Ad esempio, le immagini che sono già **lineari per scene** in genere non devono essere convertite, ad esempio le immagini **con intervallo altamente dinamico** archiviate in formati quali **OpenEXR** e **HDR**.
* Per le immagini create per la visualizzazione (**con riferimenti di visualizzazione**) sarà necessario rimuovere la gamma. Questi includono la maggior parte dei formati come **PNG**, **JPEG** e **BMP**. Queste immagini sono di **base** **colore**, **diffusione**, **specular** e **emissivo**.

Anche se si tratta di una semplificazione eccessiva, può essere utile pensare al processo come segue:

* &quot;riferiti alla scena (es. linear)&quot;: non applicare una conversione
* &quot;display-reference (es. sRGB)&quot; : applica la Trasforma inversa per &quot;linearizzare&quot; l&#39;immagine ai fini di un corretto calcolo

>[!NOTE]
>
> La funzione di decodifica sRGB (EOTF), che converte lo spazio gamma in spazio lineare, viene utilizzata in Substance Painter e Substanci Designer secondo lo standard IEC 61966-2-1:1999

È possibile configurare il Substance Designer per l&#39;utilizzo di [OpenColorIO](https://opencolorio.org/) per la gestione del colore. Ciò consente di avere *trasformazioni di colore* coerenti e la visualizzazione dell&#39;immagine in più applicazioni. In questa modalità, Substance Designer funzionerà internamente con **colori RGB lineari**. Poiché 8 profondità di bit non sono in genere sufficienti per rappresentare i colori lineari, si consiglia di utilizzare *almeno* profondità a **16 bit** per le texture di colore nel [grafico](https://docs.substance3d.com/display/SDDOC/Graph+View).

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sd-cm?$png$&jpegSize=200&wid=686)

Quando abbiamo introdotto [ACE](https://www.oscars.org/science-technology/sci-tech-projects/aces), ora abbiamo due diversi spazi cromatici, l&#39;sRGB lineare (la versione senza gamma di sRGB) e l&#39;[ACEScg](https://acescolorspace.com/), che è uno spazio cromatico ad ampia gamma (&quot;con riferimento alla scena&quot; o lineare) più adatto per il rendering CG.

*Grafica del grafico del gamut -<https://acescolorspace.com/>*

Il Substance Designer supporta anche **Adobe Color Engine (ACE)**. Con **ACE**, puoi scegliere il tuo spazio colore di lavoro tra **sRGB**, **sRGB lineare** e **ACEScg**. Quando si utilizza **sRGB**, **ACE** è simile alla modalità precedente. Quando si utilizza uno spazio colore lineare, **ACE** è più o meno simile a [OpenColorIO](https://opencolorio.org/index.html).

## Plug-in Substance

Quando si utilizza il materiale Substance tramite il plug-in di integrazione Substance, le uscite vengono contrassegnate automaticamente per i valori lineari/gamma tramite l&#39;integrazione e la gestione del colore dell&#39;applicazione host. Tuttavia, è importante comprendere a fondo il processo: quando le mappe Substance vengono utilizzate come bitmap esportate anziché come materiali Substance, potrebbe essere necessario contrassegnare manualmente le texture come **codificate con gamma** o **raw**, a seconda del modulo di rendering in uso. Di solito i file .png, .jpg, .tga o .tif a 8 o 16 bit hanno una codifica gamma, mentre i file **sRGB OETF** e .exr sono lineari.

## Applicazioni 3D

### Utilizzo della Texture

* [Substance texture in Maya](../../renderers/color-management/textures-in-maya/substance-textures-in-maya.md)
* [Substance texture in 3ds Max](../../renderers/color-management/textures-in-3ds-max/substance-textures-in-3ds-max.md)
