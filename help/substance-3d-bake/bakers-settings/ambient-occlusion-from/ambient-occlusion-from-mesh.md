---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ""
description: Esegue i baking texture di occlusione ambientale accurate da trame ad alto poli utilizzando tecniche di raytracing per un maggiore realismo.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Occlusione ambientale dalla trama
user-guide-description: ""
user-guide-title: ""
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%
---

# Occlusione ambientale dalla trama

L&#39;Occlusione Ambiente da mesh baker consente di cuocere una texture di Occlusione Ambiente da mesh poly alte. È più lento rispetto al fornello [occlusione ambiente](../../bakers-settings/ambient-occlusion/ambient-occlusion.md) di base ma produce risultati più precisi.

**Disponibile in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parametri

| *Parametro* | *Descrizione* |
| --- | --- |
| **Raggi secondari** | Quantità di raggi di occlusione. Un valore elevato produce meno rumore ma richiede più tempo per il calcolo. Il valore predefinito è 64. |
| **Distanza minima occlusione** | Distanza minima alla quale i raggi di occlusione colpiscono la geometria poly elevata. Il valore predefinito è 0,00001. |
| **Distanza massima occlusione** | Distanza massima alla quale i raggi di occlusione colpiscono la geometria poly elevata. Il valore predefinito è 0,1. |
| **Rispetto al rettangolo di selezione** | Se questa opzione è attivata, le unità sono relative al rettangolo di selezione dell’oggetto (1,0 è la lunghezza diagonale del rettangolo di selezione). Se è disattivata, le unità utilizzate per le distanze minime e massime dell’occluder sono quelle definite durante l’esportazione della trama (metri, centimetri o qualsiasi unità sia la scena esportata). |
| **Angolo di diffusione** | Angolo di estensione massimo dei raggi di occlusione. Il valore predefinito è 180. |
| **Distribuzione** | Distribuzione angolare dei raggi di occlusione. Definisce la modalità di dispersione dei raggi all’interno di un cono delle dimensioni dell’angolo di diffusione.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Coseno</strong> (impostazione predefinita): realistico ma può portare a una linea bianca in aree occluse molto sottili. Più adatto per ombreggiatura e illuminazione.</li><li data-preserve-html="true"><strong>Uniforme</strong>: utile per creare sfumature lineari. Più adatto per la mascheratura dei livelli e altri filtri.</li></ul> |
| **Ignora carattere di sfondo** | Questi parametri definiscono se i raggi di occlusione ignorano i colpi su una superficie posteriore (se la normale poly alta è orientata nella direzione opposta a quella del poly basso da cui viene sparato il raggio). Nella maggior parte dei casi questa impostazione deve essere abilitata per evitare artefatti. Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nevers</strong> (impostazione predefinita): i backface non vengono mai ignorati</li><li data-preserve-html="true"><strong>Sempre</strong>: i backface vengono sempre ignorati</li><li data-preserve-html="true"><strong>Per nome trama</strong>: le superfici posteriori vengono ignorate solo per le trame che corrispondono alla parola chiave suffisso. Consulta i [parametri comuni](../../bakers-settings/common-parameters/common-parameters.md).</li></ul> |
| **Occlusione autonoma** | Corrispondenza del nome per i raggi di occlusione. Indica in che modo i forni devono corrispondere alla geometria bassa e alta. Può essere utilizzato per filtrare il processo di cottura al forno senza la necessità di spostare manualmente (esplodere) le trame.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (impostazione predefinita): la trama a basso poli corrisponde a ogni trama a elevato poli.</li><li data-preserve-html="true"><strong>Per nome trama</strong>: filtrate le trame in base al nome per evitare che corrispondano a geometria indesiderata.</li></ul>Per ulteriori informazioni sulla geometria corrispondente, vedere: [Corrispondenza per nome](../../features/matching-by-name/matching-by-name.md). |
| **Mappa normale** | Percorso facoltativo di una texture normale. Può essere utilizzato per sostituire il calcolo interno del baker. |
| **Spazio Mondiale** | Se questa opzione è attivata, la texture normale viene interpretata come una normale spazio mondo anziché come uno spazio tangente. |
| **Orientamento normale** | Formato della texture Normale se in Spazio tangente.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (impostazione predefinita)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **Attenuazione** | Definisce la modalità di attenuazione dell&#39;occlusione in base alla distanza dell&#39;occluder.Valori possibili:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nessuno</strong>: nessuna attenuazione.</li><li data-preserve-html="true"><strong>Lineare</strong> (impostazione predefinita): attenuazione progressiva.</li><li data-preserve-html="true"><strong>Uniforme</strong>: attenuazione morbida.</li></ul> |
| **Piano terreno** | Se questa opzione è abilitata, simulate un piano sotto il rettangolo di selezione della trama sull&#39;asse XZ per entrare in collisione con i raggi secondari. Questo simula l&#39;ombra proveniente da una planimetria invisibile. |
| **Scostamento piano terreno** | Consente di allontanare il piano dalla trama per ridurre l’intensità dell’effetto. Il valore è assoluto e non relativo alla dimensione della trama. |
