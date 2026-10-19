---
helpx_url: 'https://helpx.adobe.com/it/substance-3d-general/ecosystem/general-system-requirements.html'
breadcrumb-title: ''
description: Verifica i requisiti di sistema per le applicazioni Substance 3D per assicurarti che l'hardware soddisfi le specifiche minime, consigliate o ottimali.
helpx_creative_field: ''
helpx_description: General Knowledge > Ecosystem > General system requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Requisiti generali di sistema
user-guide-description: ''
user-guide-title: ''
source-git-commit: eef3d78f33034f2c24f4c4471d9ccac805184525
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 2%
---

# Requisiti generali di sistema

## Requisiti hardware

+++Windows

|  | Minimo | Consigliato | Ottimale |
| --- | --- | --- | --- |
| **SO** | Windows 11 64 bit versione 23H2 | Windows 11 64 bit versione 24H1 | Windows 11 64 bit versione 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Archiviazione** | SSD con 30 GB di spazio disponibile | SSD con 50 GB di spazio disponibile | SSD con 70 GB di spazio disponibile |

+++

+++macOS

|  | Minimo | Consigliato | Ottimale |
| --- | --- | --- | --- |
| **SO** | Sequoia di macOS 15 | macOS 27 Golden Gate | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Archiviazione** | SSD con 30 GB di spazio disponibile | SSD con 50 GB di spazio disponibile | SSD con 70 GB di spazio disponibile |

>[!WARNING]
>
> Per le pipeline create tenendo presente la [piattaforma di riferimento VFX](https://vfxplatform.com/), le applicazioni Substance 3D possono comunque essere installate in macOS 14 Sonoma. Tuttavia, le app di Substance non sono più testate su versioni del sistema operativo inferiori ai requisiti minimi di sistema, quindi non è garantita la stabilità. Si consiglia di eseguire l’aggiornamento a una versione più recente del sistema operativo.

+++

+++Linux

|  | Minimo | Consigliato | Ottimale |
| --- | --- | --- | --- |
| **SO** | **Enterprise ETLA** RHEL 8.6 o versione successiva oppure RHEL 9.2 o versione successiva **Steam** Ubuntu 22.04.1 LTS | **Enterprise ETLA** RHEL 8.6 o versione successiva oppure RHEL 9.4 o versione successiva **Steam** Ubuntu 22.04.1 LTS o versione successiva | **Enterprise ETLA** RHEL 8.6 o versione successiva oppure RHEL 9.4 o versione successiva **Steam** Ubuntu 22.04.1 LTS o versione successiva |

**Red Hat Enterprise Linux (RHEL) 9.x**: il pacchetto xcb-util-cursor richiesto dalle nostre applicazioni è stato rimosso dal repository EPEL 9 il 10 maggio 2024. A partire da questa data, il pacchetto è supportato dal repository predefinito RHEL 9, in coincidenza con il rilascio di RHEL 9.4. I clienti che utilizzano versioni di RHEL precedenti alla 9.4 non saranno più in grado di procurarsi il pacchetto xcb-util-cursor dal repository EPEL 9 dopo il 10 maggio 2024.

Per ulteriori informazioni sulla disponibilità del pacchetto nel repository predefinito RHEL 9, consultare: [Red Hat Enterprise Linux 9 - Manifesto pacchetto - Repository AppStream](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html-single/package_manifest/index#AppStream-repository)

Per ulteriori informazioni su questa modifica, consultare: [Red Hat Bugzilla - Bug 2238273](https://bugzilla.redhat.com/show_bug.cgi?id=2238273) , [Red Hat Bugzilla - Bug 2212302](https://bugzilla.redhat.com/show_bug.cgi?id=2212302)

+++

+++VR

| Marchio | Modelli |
| --- | --- |
| Meta | Rift, Rift S, Quest, Quest 2 (con collegamento), Quest Pro |

+++

Per maggiori dettagli, esamina i requisiti di ogni applicazione:

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/sa-appicon-noshadow-256.png" alt="Icona Substance 3D Sampler" width="64px"/><br><a href="https://experienceleague.adobe.com/it/docs/substance-3d-sampler/using/getting-started/system-requirements">Substance 3D Sampler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/ds-appicon-noshadow-256.png" alt="Icona Substance 3D Designer" width="64px"/><br><a href="https://experienceleague.adobe.com/it/docs/substance-3d-designer/using/getting-started/system-requirements">Substance 3D</a> <a href="https://experienceleague.adobe.com/it/docs/substance-3d-designer/using/getting-started/system-requirements">Designer</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/pt-appicon-noshadow-256.png" alt="Icona Substance 3D Painter" width="64px"/><br><a href="https://experienceleague.adobe.com/it/docs/substance-3d-painter/using/getting-started/system-requirements">Substance 3D Painter</a></td>
  </tr>
</table>

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/md-appicon-noshadow-256.png" alt="Icona Substance 3D Modeler" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-modeler/getting-started/system-requirements.html">Substance 3D Modeler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/sg-appicon-noshadow-256.png" alt="Icona Substance 3D Stager" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-stager/getting-started/system-requirements.html">Substance 3D Stager</a></td>
    <td style="border: 0;" valign="top"></td>
  </tr>
</table>

## Note aggiuntive

### Configurazione non supportata

* Le configurazioni di computer Apple con eGPU e GPU installate dall’utente non sono supportate.
* Le macchine virtuali Windows non sono supportate.
* Il sistema operativo del server Windows non è supportato.
