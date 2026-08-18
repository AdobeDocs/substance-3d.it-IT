---
helpx_url: "https://helpx.adobe.com/it/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: Utilizzate la memorizzazione nella cache della geometria per conservare i dati di mesh pre-elaborati e velocizzare notevolmente le successive operazioni di cottura.
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Cache geometria
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Cache geometria

Durante la cottura, le trame vengono pre-elaborate per pulirle e convertite in un formato compatibile con il processo di cottura. La cache della geometria consente di conservare questa geometria pre-elaborata in modo da ricaricarla rapidamente per evitare di ripetere questa operazione in un secondo momento (a meno che la mesh di origine non cambi).

* In **Substance Designer** la cache della geometria viene creata dopo l&#39;esecuzione di un primo bake. La cache viene quindi mantenuta in memoria fino alla chiusura della finestra del baker.
* In **Substance Painter** la cache della geometria viene salvata come file con estensione **assbin** accanto al file di origine dopo il primo bake.

Il riutilizzo della cache della geometria accelera notevolmente il processo di cottura, specialmente quando si modificano le impostazioni del forno per ottenere un risultato perfetto.
