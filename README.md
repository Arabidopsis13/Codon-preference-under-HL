# Codon-preference-under-HL
R script for codon usage changes in chloroplasts under HL stress

### Polska wersja (README.md)
# Analiza użycia kodonów w genach chloroplastowych w warunkach stresu świetlnego

To repozytorium zawiera skrypt analityczny napisany w języku R, którego celem jest porównanie preferencji kodonowych w genach kodujących białka w chloroplastach w warunkach kontroli (LL) oraz stresu wysokiego natężenia światła (HL).

## 📂 Struktura repozytorium

- `Codon_Usage_Analysis.Rmd` – główny skrypt analityczny w formacie RMarkdown
- `raw_data/` – pliki wejściowe: sekwencje FASTA, adnotacje, dane zliczeń
- `produced_data/` – pliki wynikowe: wykresy i tabele z analizą

## 🧪 Opis analizy

- Normalizacja odczytów RNA-seq
- Zliczanie kodonów w adnotowanych sekwencjach genów
- Porównanie użycia kodonów między warunkami W0 (kontrola) a H24 (stres)
- Obliczenie log2FC, wartości p (test t-studenta) oraz korelacji Pearsona
- Wizualizacja wyników z podziałem na aminokwasy

## 🧰 Wymagane pakiety R

```{r}
install.packages(c("Biostrings", "dplyr", "readr", "tidyr", "ggplot2", "RColorBrewer"))
```

## 📜 Jak uruchomić

  Upewnij się, że foldery raw_data/ i produced_data/ znajdują się w tym samym katalogu co skrypt .Rmd

  Otwórz plik Codon_Usage_Analysis.Rmd w RStudio

  Knituj do HTML lub uruchom fragmenty ręcznie

## 📖 Kontekst

Analiza wykonana w ramach pracy magisterskiej dotyczącej translacyjnej odpowiedzi chloroplastów roślin na stres środowiskowy.
Skrypt może być wykorzystany również w innych analizach transkryptomicznych tRNA/codon usage.

### 🇬🇧 English version (README.md)

# Codon Usage Analysis in Chloroplast Genes under High Light Stress

This repository contains an R-based analysis script for comparing codon usage in chloroplast-encoded genes between control (LL) and high light stress (HL) conditions.

## 📂 Repository Structure

- `Codon_Usage_Analysis.Rmd` – main RMarkdown script
- `raw_data/` – input files: FASTA sequences, gene annotations, RNA-seq read counts
- `produced_data/` – output files: plots and codon usage tables

## 🧪 Analysis Overview

- Normalization of RNA-seq read counts
- Codon counting in annotated gene sequences
- Comparison between W0 (control) and H24 (stress) samples
- Calculation of log2 fold change, t-tests, and Pearson correlation
- Visualization of codon usage by amino acid

## 🧰 Required R Packages

```r
install.packages(c("Biostrings", "dplyr", "readr", "tidyr", "ggplot2", "RColorBrewer"))
```
## 📜 How to Run

   Make sure raw_data/ and produced_data/ folders are in the same directory as the .Rmd file

   Open Codon_Usage_Analysis.Rmd in RStudio

   Knit to HTML or run chunks manually

## 📖 Context

This script was developed as part of a Master’s thesis project focused on the chloroplast translational response to high light stress in plants.
It may also be adapted for general studies on codon usage.
