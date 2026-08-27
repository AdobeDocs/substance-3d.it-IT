---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/tangent-space.html"
breadcrumb-title: ''
description: Scopri come Substance Bakers gestisce i calcoli dello spazio tangente e personalizza l'algoritmo per il tuo flusso di lavoro.
helpx_creative_field: ""
helpx_description: bakers > Features > Tangent Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Spazio tangente
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 1%

---


# Spazio tangente

Substance Bakers può caricare le tangenti e i binomiali presenti sulla trama low-poly o ricalcolarli. Quando li ricalcoli è possibile definire un algoritmo di Spazio tangente personalizzato (per impostazione predefinita è MikkTSpace).

## Elenco dei plug-in di Spazio tangente

## Substance Painter

In Substance Painter il plug-in Tangent Space non può essere modificato, sarà sempre **MikkTSpace**. Tuttavia, esiste un parametro che ne modifica leggermente il comportamento per renderlo compatibile con altre applicazioni:

| *Parametro* | *Compatibile* *Applicazione* |
| --- | --- |
| **Calcolo dello spazio tangente per frammento: disattivato** | Compatibile con xNormal, Unity 5.3 o versioni successive. |
| **Calcolo dello spazio tangente per frammento: abilitato** | Compatibile con il flusso di lavoro Unreal Engine 4, Blender e Unity HDRP. |

## Substance Designer

Substance Designer supporta il seguente algoritmo:

| *Nome file* | *Descrizione* |
| --- | --- |
| **mikktspace.dll** | MikkTSpace, algoritmo di Spazio tangente basato sul lavoro di Morten S. Mikkelsen.Compatibile con xNormal, Unity 5.3 o versioni successive. |
| **mikkunrealtspace.dll** | MikkTSpace, algoritmo di Spazio tangente basato sul lavoro di Morten S. Mikkelsen.Compatibile con il flusso di lavoro Unreal Engine 4, Blender e Unity HDRP. |
| **unitytspace.dll** | Algoritmo di Spazio tangente basato su Unity 4. |

>[!NOTE]
>
> È possibile scrivere un plug-in personalizzato per lo spazio tangente. Un file di intestazione denominato **tangentspaceplugin.h** è disponibile nella cartella di installazione in **Substance Designer/SDK/tangentspace** e può essere utilizzato come interfaccia.

## Spazio tangente personalizzato

## Substance Painter

Al momento, Substance Painter non supporta i plug-in di Spazio tangente personalizzati. Ciò significa che se Tangenti e Binormali non sono presenti sulla trama a basso poli (utilizzata per creare il progetto) verranno ricalcolati in base all&#39;algoritmo MikkTSpace.

## Substance Designer

Per impostare l&#39;algoritmo dello spazio tangente in Substance Designer, effettuate le seguenti operazioni:

1. Scegli **Modifica** > **Preferenze**.

   ![](../../assets/sd-edit-pref.png)
1. Fai clic su **Progetti**.

   ![](../../assets/sd-pref-projects.png)
1. Passa alla scheda **Generale**. Scorrete fino a visualizzare la sezione **Scene 3D**.

   ![](../../assets/sd-tab-general.png)
1. Fai clic sui **tre punti** (...) per caricare un plug-in personalizzato.

## Substance Automation Toolkit

Quando si esegue i baking con il toolkit di automazione è possibile specificare il plug-in Tangent Space con un argomento della riga di comando specifico:

```
sbsbaker normal-from-mesh --tangent-space-plugin "C:/Substance Designer/plugins⁄tangentspace⁄mikktspace.dll" ...
```
