---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-1.html"
breadcrumb-title: ''
description: Consulta le note sulla versione per il componente aggiuntivo Blender versione 0.9.1 per scoprire le nuove funzioni, i miglioramenti e le correzioni di bug.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 0.9.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Componente aggiuntivo 0.9.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Componente aggiuntivo 0.9.1

**Note sulla versione per il componente aggiuntivo 0.91+**

* Nota: *La versione del plug-in 0.91+ non è compatibile con le versioni precedenti del plug-in!*
* Riarchitettura del codebase interno per migliorare le prestazioni e la stabilità del plug-in
* Interfaccia utente rinnovata per migliorare l’esperienza utente complessiva
* È stata aggiunta un’interfaccia utente per consentire la modifica della suddivisione in porzioni predefinita
* È stato aggiunto il supporto per l’aggiornamento delle texture nella vista di rendering dei cicli.
* È stata aggiunta la gestione degli errori nella console per notificare se il caricamento di una sostanza non è riuscito
* Menu mobile con azioni rapide aggiornato

**Sezione Preferenze: aggiunta/aggiornamento:**

* Parametro Formato immagine di esportazione; quando le immagini generate nel modulo di fusione vengono utilizzate come input di immagine per un materiale di Substance, questo formato viene utilizzato per salvare l’immagine nella cartella Temporale.
* Percorso libreria Substance; specifica la cartella aperta per impostazione predefinita quando si utilizza il pulsante Carica per cercare un file Substance.
* Percorso predefinito di esportazione delle texture (cartella Temporale) che emula il percorso utilizzato da Substance 3D Painter per gestire le esportazioni di file non salvati
* Il percorso relativo della texture è uguale a quello precedente, con la possibilità di utilizzare chiavi come $matName per creare sottocartelle
* Percorso dei file Sbsar relativo alla creazione di una sottocartella che raccoglie i file sbsar utilizzati nel file di fusione quando si salva il progetto
* Possibilità di impostare dinamicamente diverse reti di shader nelle preferenze - Nella rete di shader, possibilità di impostare diverse variabili per shader a seconda delle esigenze dello shader
* Nella sezione output della rete shader, è possibile impostare se un output è abilitato per impostazione predefinita
* Possibilità di impostare lo spazio colore (che supporta i flussi di lavoro cinematografici aces, linear exr e blender, non solo srgb)
* Selezione predefinita del formato immagine e della profondità di bit
* Un output generico per impostare i valori per gli utilizzi di output non definiti nello shader, ad esempio se si dispone di un altro output non utilizzato per impostazione predefinita dallo shader, ad esempio come una maschera.
* Un filtro per cambiare il tipo di output (1 solo output abilitato, 2 tutti gli output che si trovano nello shader e nella Substance, 3 tutti gli output disponibili nella Substance)
* Supporto per scelte rapide personalizzate (modificate)

**Sezione del pannello Substance 3D: aggiunta/aggiornamento:**

* Possibilità di regolare e bloccare il valore dei parametri di Affiancamento e risoluzione
* Interfaccia utente predefinita aggiornata: il menu a discesa del tipo di shader per modificare il tipo di grafico che gli utenti desiderano avere
* È stato modificato il parametro di input dell’immagine nello standard utilizzato in Blender. Ora puoi utilizzare le immagini di fusione e non solo i file
* Possibilità di lavorare in più istanze di Blender in qualsiasi momento
* Supporto per l’evidenziazione automatica dei materiali nel pannello Substance 3D quando il materiale è selezionato nella finestra della vista
