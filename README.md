# Charge-driven antiviral responses enhance autoreactivity in severe COVID-19

This repository contains the analysis code accompanying the manuscript **"Charge-driven antiviral responses enhance autoreactivity in severe COVID-19"** (Witman et al., submitted to *Nature Communications*).

## Repository contents

- `Polyreactivity_COVID.Rmd` — R Markdown file containing all analysis code used to generate the figures and statistical results reported in the manuscript and supplemental figures.

## Data availability

All data files required to run this code are deposited on figshare:
**https://doi.org/10.6084/m9.figshare.32836157**

File paths in the current version of the R Markdown script point to local directories used during development. To reproduce the analysis, download the corresponding files from the figshare link above and update the file paths in each code chunk to point to your local copy.

Additional deposited data:
- scRNA-seq and paired V(D)J-seq datasets: NCBI BioProject accession **PRJNA1391649**

## Analysis overview

The R Markdown file is organized into chunks corresponding to distinct stages of the analysis:

| Chunk | Description |
| --- | --- |
| ANA Score information | ANA ELISA scoring and group comparisons (Figure 1A; Supplemental Figure 1) |
| ANA IF analysis | Immunofluorescence staining pattern analysis (Figure 1B, C) |
| ELISA analysis | Polyreactivity and antiviral ELISA processing (Figure 2A, B) |
| AbMap paratope analysis | Paratope similarity embedding and UMAP analysis (Figure 3C–E) |
| Monoclonal Information Assignment | Compilation of monoclonal antibody metadata |
| Germlines Generation of Highly Reactive Clones | Germline reversion of selected clones |
| Generating Features of HCDR3s of High Clones | HCDR3/LCDR3 charge and composition analysis (Figure 4A–C; Supplemental Figure 2A) |
| Generating Structural Figures | Docking structure visualization (Figure 4D–F) |
| Calculating Interface Charge | Interface charge/PDBePISA-based analysis (Table 1) |
| Antibody mutants analysis | Charge mutant ELISA binding comparisons (Figure 5E, F) |
| Germline vs Patient derived analysis | Germline-to-patient AUC binding comparisons (Figure 5A–D; Supplemental Figure 3) |
| Reverting Germline Clones from Other Sources | Germline reconstruction for additional clone sets |
| Generating GermvsPat Charge Ratios | Charge change calculations across CDRs |
| Identifying High Clones | Selection of top-reactivity clones (Supplemental Table 1) |
| Converting PDBePISA XMLs | Parsing of PDBePISA interface output files |
| Making Trees | Clonal lineage tree reconstruction (Figure 2D) |
| Spike used in ELISA charge changes | Spike/variant charge calculations (Figure 6A; Table 2; Supplemental Figure 4A, B) |
| Competitive RBD ELISA | RBD competition ELISA analysis |
| Influenza Analysis | Hemagglutinin repertoire charge analysis (Figure 7F, G) |

## Requirements

Analyses were performed in R. The following packages are required:

`Biostrings`, `FNN`, `FSA`, `Seurat`, `airr`, `alakazam`, `bio3d`, `broom`, `dendextend`, `dowser`, `dplyr`, `fields`, `forcats`, `ggbeeswarm`, `ggdendro`, `ggdist`, `ggplot2`, `ggpubr`, `ggrepel`, `ggtext`, `ggtree`, `grid`, `gt`, `httr`, `openxlsx`, `patchwork`, `pheatmap`, `pracma`, `purrr`, `pwalign`, `readr`, `readxl`, `rentrez`, `rstatix`, `shazam`, `stringdist`, `stringr`, `tibble`, `tidyr`, `tidyverse`, `writexl`, `xml2`

## Contact

For questions, or if a data file, script, or figure cannot be located, please reach out:

- Nathan Witman — NAW271@pitt.edu
- Renren Wen (corresponding author) — rwen@versiti.org
