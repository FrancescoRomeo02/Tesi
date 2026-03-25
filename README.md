# Tesi di Laurea Magistrale in Informatica

Questo repository contiene il codice sorgente LaTeX per la tesi di Laurea Magistrale in Informatica presso l'**Università degli Studi di Milano-Bicocca**.

## Dettagli

- **Candidato:** Francesco Romeo (Matricola: 885880)
- **Relatrice:** Dott.ssa Elisabetta Fersini
- **Co-relatore:** Dottor Marco Loregian
- **Anno Accademico:** 2025/2026

## Struttura del Progetto

Il progetto è strutturato in diversi file e cartelle per mantenere il codice LaTeX organizzato:

- `main.tex`: File principale da compilare che aggrega tutti i capitoli e le impostazioni.
- `preface/`: Contiene l'introduzione alla tesi.
- `chapterX/`: Cartelle contenenti i file `.tex` dei singoli capitoli (da 1 a 5).
- `conclusions/`: Contiene il capitolo relativo alle conclusioni e agli sviluppi futuri.
- `appendices/`: Contiene le appendici della tesi (convenzioni matematiche, listati di codice, ecc.).
- `bibliography/`: Contiene il file `bibliography.bib` con i riferimenti bibliografici gestiti tramite `biblatex`.
- `logos/`: Immagini per il frontespizio, come il logo dell'università.
- `thankyou/`: Sezione per i ringraziamenti.

## Requisiti e Compilazione

Il documento sfrutta diversi pacchetti standard di LaTeX (inclusi `amsmath`, `graphicx`, `biblatex`, `hyperref`, e pacchetti per la localizzazione in italiano come `babel`).

Per compilare correttamente il documento e generare il file `main.pdf` completo di bibliografia e indice, si raccomanda l'uso di uno strumento come `latexmk` che automatizza le passate di compilazione, per esempio:

```bash
latexmk -pdf main.tex
```

In alternativa, se si vuole procedere con la compilazione manuale (usando `pdflatex` e `biber`):

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

## Note

Le macro matematiche personalizzate (come quelle per le parentesi scalabili e colori specifici dell'università) e lo stile delle intestazioni (`mystyle` usando il pacchetto `fancyhdr`) sono definiti direttamente nel preambolo del file `main.tex`.
