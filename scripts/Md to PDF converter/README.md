---
source-git-commit: a517442244806bc6aef0f5bfb165c5d4f67341be
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---
# Markdown al convertitore PDF

Questa cartella contiene uno script di preelaborazione e conversione per la generazione di versioni PDF delle pagine della documentazione da questo repository.

## Perché questo esiste

I file di origine della documentazione utilizzano una sintassi di markdown specifica per la piattaforma Adobe (blocchi di fisarmonica, didascalie di avviso ed estensioni di attributi immagine) non compresa dagli strumenti di markdown standard. Questo script normalizza la sintassi e converte il file in PDF utilizzando [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf), comprimendo le immagini per mantenere gestibili le dimensioni del file di output.

## Prerequisiti

- [Node.js](https://nodejs.org/) (v18 o versioni successive)
- Le dipendenze sono già installate in `node_modules/`. Se devi reinstallarli, esegui `npm ci` da questa cartella.

## Utilizzo

Eseguire lo script dalla **directory principale del repository**, passando il percorso al file di markdown da convertire:

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" <path/to/file.md>
```

**Esempio:**

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" help/substance-3d-general/openpbr/openpbr-overview.md
```

Il PDF viene scritto nella **stessa directory del file di origine**. I file temporanei creati durante la conversione (`*.pdf-ready.md` e `_pdf-images/`) vengono eliminati automaticamente al termine dell&#39;operazione. Se la conversione non riesce, vengono lasciati in posizione per facilitare il debug.

## Funzionamento dello script

| Sintassi di origine | Uscita PDF |
|---|---|
| `+++Title` / `+++` blocchi accordion | Intestazione `#####` con contenuto sempre visibile |
| Callout avvisi di `>[!NOTE]` | Virgoletta standard con prefisso **Nota:** in grassetto |
| `![](path){width="N"}` attributi immagine | Il tag `<img>` mantiene la larghezza specificata |
| Collegamenti immagine markdown a `.pdf` file | Rimosso (riferimenti per il download automatico solo per il Web) |
| `hold:` chiave di frontmatter | Rimosso (metadati solo piattaforma) |
| Tutte le immagini | Ridimensionato a una larghezza massima di 1200 px, codificato nuovamente come JPEG con una qualità dell’80% |
| Tutte le tabelle | Bordi e sfondi rimossi tramite CSS inserito |
