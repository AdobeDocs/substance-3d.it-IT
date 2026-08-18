---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: Scoprite quando abilitare Calcola spazio tangente per frammento e come influisce sui risultati di cottura.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Should I enable
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: È necessario abilitare
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---


# È necessario abilitare &quot;Calcola spazio tangente per frammento&quot;?

>[!WARNING]
>
> **Domanda**
> 
> Cosa significa l&#39;impostazione &quot;Calcola spazio tangente per frammento&quot; e qual è l&#39;utilizzo?

>[!NOTE]
>
> **Spiegazione**
> 
> Quando attivata, questa impostazione indica al fornaio di eseguire il calcolo dello spazio tangente in Shader frammento (detto anche Pixel Shader) anziché in Shader vertice. Significa che il calcolo verrà eseguito per pixel invece di essere interpolato da un vertice all’altro. Queste impostazioni vengono utilizzate dal normale baker di mappe per sapere come codificare la texture. Sapeva anche come leggere la texture dagli shader.
> 
> L’attivazione o la disattivazione di questo parametro richiede in genere di rieseguire il rendering delle texture per sincronizzarle con le finestre delle viste 3D e i motori di rendering (ad esempio Iray).

>[!NOTE]
>
> **Soluzione**
> 
> A seconda del software o del motore di gioco utilizzato per eseguire il rendering della texture, questa impostazione può essere disattivata o attivata:
> 
> | *Software* | *Calcolare lo spazio tangente per frammento* |
> | --- | --- |
> | **Motore irreale 4** | Attivato |
> | **Unità** | Disattivato |
