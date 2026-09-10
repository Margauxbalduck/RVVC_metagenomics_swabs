# RVVC Vaginal Microbiome Analysis

This repository contains the R/Quarto analysis code associated with the study:

**Clinical Severity Associates with Host-Microbiome States in Recurrent Vulvovaginal Candidiasis**

## Overview

This study investigates the vaginal microbiome in women with recurrent vulvovaginal candidiasis (RVVC) and healthy controls using shotgun metagenomic sequencing.

The analyses examine associations between vaginal microbial composition and functional potential, *Candida albicans*, clinical disease severity, and host mucosal responses.

## Analyses

The Quarto (.qmd) files contain the taxonomic and functional microbiome analyses used in the study, with separate workflows for microbial community composition and microbial functional potential, including:

* Microbial taxonomic composition
* Alpha and beta diversity
* Differential abundance
* Community state type (CST) classification
* Associations with clinical severity
* Microbial functional pathway analysis
* Microbiome co-abundance analyses
* Integration with host transcriptomic data
* Integration with CD66b immunofluorescence staining data
* Generation of manuscript figures and tables

## Project structure

The repository contains two main Quarto (`.qmd`) analysis files:

```text
RVVC_metagenomics_swabs/
├── 01_vvc_microbiome_analysis.qmd
├── 02_rvvc_functional_analysis.qmd
└── README.md
```

### `01_vvc_microbiome_analysis.qmd` — Taxonomic microbiome analysis

Contains the main taxonomic analyses of the vaginal microbiome based on shotgun metagenomic sequencing data. Analyses include:

* Data preprocessing, sample selection, filtering, and normalization
* Alpha and beta diversity analyses
* ANOSIM and PERMANOVA
* Differential abundance analysis using ALDEx2
* Relative abundance and major bacterial species analyses
* Lactobacillus abundance analyses
* Community state type (CST) classification
* Microbial composition heatmaps
* Associations with *Candida* detection
* Associations between microbial composition and clinical severity
* Clinical-score-stratified diversity and differential abundance analyses
* Integration with clinical and medical history data
* Microbial co-abundance/network analyses
* Generation of taxonomic figures and summary tables

### `02_rvvc_functional_analysis.qmd` — Functional microbiome analysis

Contains analyses of the functional potential of the vaginal microbiome based on microbial pathway abundance data. Analyses include:

* Functional pathway data preprocessing, quality control, filtering, and normalization
* Differential pathway abundance analysis using ALDEx2
* Alpha and beta diversity of functional profiles
* ANOSIM and PERMANOVA of functional composition
* Cross-sectional comparisons between study groups
* Associations between functional profiles and clinical severity
* Integration of functional profiles with host transcriptomic clustering
* Pathway abundance heatmaps and participant-level visualizations
* Species contributions to microbial pathways
* Grouping of pathways into higher-level biological pathway classes (MetaCyc superclasses)
* Superclass-level diversity, differential abundance, and statistical analyses
* Correlations between pathway functions and clinical severity
* PCoA analyses with functional pathway and superclass overlays
* Generation of functional microbiome figures and summary analyses

## Data availability

Raw metagenomic sequencing data will be deposited in the European Nucleotide Archive (ENA).

Processed taxonomic and functional pathway data are provided with the associated manuscript where applicable.

Participant-level clinical data are not publicly available due to the sensitive nature of these data.

## Software

Analyses were primarily performed in **R** and documented using **Quarto**.

Package requirements and analysis-specific dependencies are described within the individual analysis files.

## Repository status

This repository accompanies an ongoing manuscript and may be updated during manuscript preparation and peer review.

## Citation

Citation information will be added following publication.

## Contact
For questions regarding the analyses or this repository, please contact:

Margaux Balduck
Department of Medicine Solna, Division of Infectious Diseases
Karolinska Institutet
Stockholm, Sweden
Email: margaux.balduck@ki.se

