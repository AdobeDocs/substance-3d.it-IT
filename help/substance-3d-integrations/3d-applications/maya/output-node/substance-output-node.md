---
helpx_url: "https://helpx.adobe.com/it/substance-3d-integrations/3d-applications/maya/substance-output-node.html"
breadcrumb-title: ''
description: Informazioni sul funzionamento dei nodi di output Substance in Maya per connettere le texture calcolate alle reti shader.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance Output Node
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance nodo di output
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Substance nodo di output

Il nodo di output della Substance è un riferimento alla texture calcolata dalla Substance Engine. È connesso al nodo Substance. Quando viene creato un output sul nodo della Substance, il modulo di gestione della Substance calcola la texture e questi dati vengono mantenuti nella RAM. Se si utilizza il motore GPU, i dati vengono calcolati sulla GPU e inviati di nuovo in memoria utilizzando il motore di fusione GPU Substance. Gli output sul nodo Substance non attivati non vengono calcolati.

![](../../../assets/outputnode.png)

In questo nodo, è possibile visualizzare informazioni di output quali l&#39;identificatore, l&#39;etichetta e l&#39;utilizzo impostati sull&#39;output in Substance Designer. Questo nodo consente inoltre di eseguire il batch della texture su disco nella sezione Memorizzazione nella cache di output.
