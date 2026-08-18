---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: Risoluzione dei problemi relativi al motivo per cui le texture create al di fuori del software Substance non sono corrette e come risolvere i problemi di spazio colore.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La texture creata al di fuori del software Substance non sembra corretta
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# La texture creata al di fuori del software Substance non sembra corretta

>[!WARNING]
>
> **Domanda**
> 
> Perché la texture che ho preparato con un&#39;applicazione esterna e non con Substance Bakers ha un aspetto errato nella Substance Painter?

>[!NOTE]
>
> **Soluzione**
> 
> Non esiste una soluzione immediata a questo problema, in quanto molti fattori possono contribuire a risolvere il problema:
> 
> * Verificare che il formato normale tra il software di Substance e l&#39;applicazione esterna sia lo stesso. OpenGL è [X+, Y+, Z+] e DirectX è [X+, Y-, Z+]
>   * In Substance Painter è possibile modificare il formato normale nella [configurazione del progetto](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/project-configuration).
>   * In Substance Designer il formato normale può essere modificato nelle [preferenze del progetto](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings).
> * Verificare che la trama sia stata triangolata prima della cottura al forno e dell&#39;importazione nel software di Substance. Per ulteriori informazioni, vedere [questa pagina](../../guides/triangulating-before-bak/triangulating-before-baking.md).
