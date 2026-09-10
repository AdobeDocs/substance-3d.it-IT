---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity.html"
breadcrumb-title: ''
description: Importa e utilizza i materiali Substance nel motore di gioco Unity con supporto nativo dei plug-in e controllo dei parametri di runtime.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unità
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# Unità

![](../../assets/unity.png)

>[!NOTE]
>
> **Versioni supportate dall&#39;unità**
> 
> Il plug-in Substance 3D per Unity versione 3.0.0 attualmente supporta Unity 2020.3.27x e versioni successive. È possibile scaricarla dall&#39;[Archivio risorse di Unity](https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208).

>[!WARNING]
>
> Prima di eseguire l&#39;aggiornamento o di utilizzare il plug-in, controllare la [pagina di aggiornamento del progetto](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html).

>[!WARNING]
>
> Verificare la pagina [Linee guida per l&#39;ottimizzazione](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) prima di creare materiali di Substance personalizzati.

## Sommario

* [Note sulla versione di Unity](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Novità della versione di Substance del plug-in Unity
* [Download del plug-in Substance 3D in Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — Adobe Substance 3D for Unity è disponibile nell&#39;archivio risorse di Unity https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555.
* [Panoramica del plug-in di unità](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Preferenze unità](../../game-engines/unity/unity-preferences/unity-preferences.md): la finestra Substance preferenze consente di impostare le opzioni definite dall&#39;utente per il plug-in.
* [Linee guida per l&#39;ottimizzazione](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md): durante la creazione di materiali di Substance personalizzati, verificare le seguenti linee guida per l&#39;ottimizzazione.
* [Aggiornamento di progetti/problemi noti](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — Problemi noti con la Substance nel plug-in Unity
* [Gestione dei Grafici Substance](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html): è possibile creare nuovi materiali in base al materiale di Substance utilizzando Gestione Grafici Substance (SGM)
* [Modifica dei parametri](../../game-engines/unity/changing-parameters/changing-parameters.md) - I parametri per il materiale della Substance sono accessibili sull&#39;oggetto Grafico Substance (SGO).
* [Texture generate (Impacchettamento)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md): le Texture generate mostrano gli output della Substance calcolati dalla Substance Engine per creare texture
* [Rendering dello spazio colore](../../game-engines/unity/rendering-color-space/rendering-color-space.md): per risultati ottimali, imposta lo spazio colore su lineare in Impostazioni lettore Unity.
* [Utilizzo degli input dell&#39;immagine](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [Pubblicazione per dispositivi mobili](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) — Linee guida per la pubblicazione su piattaforme mobili
* [Scripting per Substance 3D for Unity](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md): mediante l&#39;API Substance, è possibile scrivere script per aggiornare e modificare i parametri Substance in fase di esecuzione.
* [Scripting in Unity (deprecato)](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Utilizzando l&#39;API Substance, è possibile scrivere script per aggiornare e modificare i parametri Substance in fase di runtime.
* [Utilizzo libreria Substance 3D Assets](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Rimozione del plug-in Substance](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D in Unity Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Dimensioni fisiche nell&#39;unità](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
* [Condivisione di file sbsar tra progetti](https://helpx.adobe.com/sharing-sbsar-files-between-projects.html)[](../../game-engines/unity/sharing-sbsar-files-bet/sharing-sbsar-files-between-projects.md)

**[MODULO TROVATO - REGOLE OBBLIGATORIE]**

>[!WARNING]
>
> Prima di eseguire l&#39;aggiornamento o di utilizzare il plug-in, controllare la [pagina di aggiornamento del progetto](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html).

>[!WARNING]
>
> Verificare la pagina [Linee guida per l&#39;ottimizzazione](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) prima di creare materiali di Substance personalizzati.

### Sommario

* [Note sulla versione di Unity](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Novità della versione di Substance del plug-in Unity
* [Download del plug-in Substance 3D in Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — Adobe Substance 3D for Unity è disponibile nell&#39;archivio risorse di Unity https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555.
* [Panoramica del plug-in di unità](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Preferenze unità](../../game-engines/unity/unity-preferences/unity-preferences.md): la finestra Substance preferenze consente di impostare le opzioni definite dall&#39;utente per il plug-in.
* [Linee guida per l&#39;ottimizzazione](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md): durante la creazione di materiali di Substance personalizzati, verificare le seguenti linee guida per l&#39;ottimizzazione.
* [Aggiornamento di progetti/problemi noti](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — Problemi noti con la Substance nel plug-in Unity
* [Gestione dei Grafici Substance](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html): è possibile creare nuovi materiali in base al materiale di Substance utilizzando Gestione Grafici Substance (SGM)
* [Modifica dei parametri](../../game-engines/unity/changing-parameters/changing-parameters.md) - I parametri per il materiale della Substance sono accessibili sull&#39;oggetto Grafico Substance (SGO).
* [Texture generate (Impacchettamento)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md): le Texture generate mostrano gli output della Substance calcolati dalla Substance Engine per creare texture
* [Rendering dello spazio colore](../../game-engines/unity/rendering-color-space/rendering-color-space.md): per risultati ottimali, imposta lo spazio colore su lineare in Impostazioni lettore Unity.
* [Utilizzo degli input dell&#39;immagine](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [Pubblicazione per dispositivi mobili](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) — Linee guida per la pubblicazione su piattaforme mobili
* [Scripting per Substance 3D for Unity](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md): mediante l&#39;API Substance, è possibile scrivere script per aggiornare e modificare i parametri Substance in fase di esecuzione.
* [Scripting in Unity (deprecato)](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Utilizzando l&#39;API Substance, è possibile scrivere script per aggiornare e modificare i parametri Substance in fase di runtime.
* [Utilizzo libreria Substance 3D Assets](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Rimozione del plug-in Substance](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D in Unity Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Dimensioni fisiche nell&#39;unità](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
