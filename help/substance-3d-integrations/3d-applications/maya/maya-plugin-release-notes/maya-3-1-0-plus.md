---
description: Consultate le note sulla versione per il plug-in Maya versione 3.0.0 e successive per informazioni sulle nuove funzioni, i miglioramenti e le correzioni di bug.
title: Maya 3.0.0
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%
---

# Maya 3.1.0+

## Maya 3.1.1

**Data di pubblicazione:** 18 novembre 2026

**Compatibile con:** Maya 2025 e versioni successive

### Aggiunto/Aggiornato

* Aggiornamento Substance Engine (9.6.1.) incluse correzioni di sicurezza
* Supporto di OpenPBR per Maya 2025, 2026 e 2027 (Arnold e V-Ray)

### Limitazioni note

* Peso di emissione: il parametro peso_emissione non fa parte della specifica di cui all&#39;OpenPBR 1.1 e non è collegato automaticamente. Dopo aver applicato il flusso di lavoro, impostate manualmente il valore Peso emissione nel nodo di OpenPBR se il materiale utilizza l&#39;emissione.
* OpenPBR - V-Ray - Subsurface Radius Scale: quando si utilizza il flusso di lavoro OpenPBR - V-Ray, subsurface_radius_scale può restituire un valore di 0. In tal caso, rimuovere la connessione e impostare manualmente il valore nel nodo V-Ray.
* Differenze visive tra i moduli di rendering: alcune variazioni tra l’anteprima del materiale in Substance 3D Designer e il risultato renderizzato in Arnold o V-Ray sono dovute alle differenze nell’implementazione della specifica OpenPBR da parte di ciascun modulo di rendering e miglioreranno con la convergenza delle implementazioni.
* File SBSAR esportati da Substance 3D Painter 12.2.0. o versioni precedenti potrebbero non collegarsi correttamente quando si utilizza un flusso di lavoro di OpenPBR Maya 3.1.0 Aggiunto/Aggiornato: Aggiornamento Substance Engine (9.6.1.) incluse correzioni di sicurezza.

## Maya 3.1.0

**Data di pubblicazione:** 18 novembre 2026

**Compatibile con:** Maya 2024

### Aggiunto/Aggiornato

* Aggiornamento Substance Engine (9.6.1.) incluse correzioni di sicurezza
