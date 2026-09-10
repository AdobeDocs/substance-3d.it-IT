---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/visual-feedback-of-animated-substances.html"
breadcrumb-title: ''
description: Abilita l’anteprima animata in Cinema 4D per visualizzare il feedback visivo dei materiali animati per Substance nella finestra della vista.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Visual Feedback of Animated Substances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Feedback visivo della Substance animata
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 3%

---


# Feedback visivo della Substance animata

Per ottenere un feedback visivo di una Substance animata nella finestra della vista di Cinema 4D, è necessario attivare l’opzione Anteprima animata per questi materiali.

Questa opzione si trova in Editor materiale sotto Editor (vedi di seguito). Se un materiale è stato creato mediante il comando Crea materiale (o materiali), questa opzione sarà attivata per impostazione predefinita.

![](../../../assets/cinema-4d-13.png){width="500px"}


## Creazione di materiali

Il comando Crea materiali in Gestione risorse Substance consente di creare in modo semplice e rapido materiali di Cinema 4D utilizzando una Substance.

Pertanto, verrà utilizzata la seguente mappatura dei canali:

|  |  |
| --- | --- |
| **Substance canale di output** | **Canale materiale Cinema 4D** |
| Diffusione | Colora |
| Con emissioni | Luminanza |
| Riflesso | Riflettenza |
| Ambiente | Ambiente |
| Rilievo | Rilievo |
| Opacità | Alfa |
| Speculare | Riflettenza/Specular predefinito |
| Altezza | Spostamento |
| Normale | Normale |

Questa relazione viene utilizzata solo per il comando Crea materiale (o materiali) e il materiale creato può essere successivamente modificato. Potete usare questo comando per creare rapidamente un materiale di base, che può quindi essere perfezionato modificando solo alcuni canali.

All’interno dello Shader della Substance non ci sono solo i pochi canali di output sopra elencati, ma potete utilizzare qualsiasi canale di output fornito da una Substance.

## Creazione manuale di materiali di Substance

Anziché utilizzare il comando Crea materiali, potete anche creare i materiali manualmente utilizzando lo shader della Substance.

È sufficiente selezionare lo shader della Substance in un canale di materiale e trascinare nella Substance che si desidera utilizzare. Il prossimo passaggio consiste nel selezionare il canale di output della Substance da utilizzare in questo shader, e hai finito.

Metti Mi piace così:

![](../../../assets/cinema-4d-15.png){width="800px"}

Questo metodo offre molta libertà creativa e consente di effettuare le seguenti operazioni:

* Assegnate i canali di output Substance ai canali di materiale Cinema 4D arbitrari. Non è necessario limitarsi a utilizzarli solo nei canali previsti.
* Assegnate un singolo canale di output Substance a diversi canali di materiale Cinema 4D.
* Assegnate i canali di output di più Substance a un singolo materiale Cinema 4D.

## Limitazioni

* I fotogrammi chiave nei parametri di input della Substance sono visualizzati nella timeline, ma non nel cursore di avvio di Cinema 4D (il cursore della timeline sotto le finestre delle viste).
* A causa di una limitazione, sui canali di output Substance non devono essere utilizzati profili colore personalizzati.
* In determinate circostanze, l&#39;input dell&#39;immagine della Substance si interrompe il\
  Comando Unisci... di Cinema 4D, che combina due scene in una sola. Ciò accade se la scena da unire si trova nella directory del progetto e gli input dell’immagine si riferiscono alle immagini nella directory del progetto. In questi casi, gli ingressi delle immagini dovranno essere ricollegati manualmente in seguito.
* Se le Substance si trovano nella cartella del progetto (o altrove nel percorso di ricerca globale), non funzionano in Cineware. In questo caso vengono visualizzati in rosso, come se la Substance fosse mancante. Per risolvere questo problema, gli archivi di Substance devono essere archiviati all&#39;esterno della directory del progetto, in modo che vi venga fatto riferimento da un percorso assoluto. È possibile utilizzare il parametro Filename per modificare la posizione del file dopo che i file sono stati spostati all’esterno del percorso del progetto.
