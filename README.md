# Institutional Justice in GBV Survivor Narratives

This repository contains the public-release analysis notebooks supporting the dissertation:

**How do gender-based violence survivors describe institutions in narratives of justice and injustice?**

## Project overview

The project examines how institutional experiences are described in interview narratives from victim-survivors of gender-based violence. It combines computational text analysis with manual annotation and targeted close reading.

The analytical workflow includes:

1. corpus preparation;
2. construction and validation of an institutional retrieval dictionary;
3. full-corpus keyword-in-context (KWIC) retrieval;
4. TF-IDF analysis;
5. non-negative matrix factorisation (NMF);
6. manual annotation sampling and analysis;
7. targeted close reading;
8. publication-oriented visualisation.

Computational methods are used for systematic retrieval and exploratory pattern identification, rather than as a replacement for qualitative interpretation.

## Repository contents

| Notebook | Description |
|---|---|
| `01_data_preparation.ipynb` | Preliminary corpus preparation and transcript extraction |
| `02_final_corpus_and_dictionary.ipynb` | Final corpus construction and institutional dictionary |
| `03_full_corpus_kwic_validation.ipynb` | Full-corpus KWIC retrieval and validation |
| `04_tfidf_analysis.ipynb` | TF-IDF analysis of transcript-category documents |
| `05_nmf_analysis.ipynb` | Exploratory NMF topic modelling and artefact screening |
| `06_annotation_sampling_design.ipynb` | Formal annotation sampling design |
| `07_manual_annotation_analysis.ipynb` | Aggregate analysis of manually annotated records |
| `08_targeted_close_reading.ipynb` | Selection framework for targeted close reading |
| `09_final_visualisations.ipynb` | Final publication-oriented figures |

## Data availability and ethics

The source interview material is sensitive qualitative research data and is not redistributed in this repository.

This public release excludes:

- interview transcripts;
- transcript excerpts and KWIC contexts;
- participant and file identifiers;
- manual annotation records;
- validation workbooks;
- close-reading case files;
- intermediate text-bearing datasets.

The notebooks are provided without saved outputs. Consequently, they cannot be executed end-to-end without authorised access to the restricted source data and intermediate files.

The source dataset is available through the UK Data Service ReShare under its applicable access and ethical conditions:

**Justice, inequality and gender-based violence project: Victim/survivors’ experiences and views of justice, 2015–2018 (ReShare record 853338).**

## Analytical scope

The final analysis used:

- 141 analytical transcripts;
- a 42-term institutional retrieval dictionary;
- 8,865 occurrence-level raw keyword hits;
- 627 transcript-by-category documents for TF-IDF;
- 588 cleaned transcript-by-category documents for the final NMF model;
- 90 formal annotation records;
- 73 valid annotated institutional mentions from 60 unique transcripts.

Raw keyword hits represent retrieval occurrences, not independent institutional experiences or prevalence estimates.

## Software

The analysis was conducted in Python using packages including:

- pandas;
- NumPy;
- scikit-learn;
- spaCy;
- Matplotlib;
- seaborn;
- openpyxl;
- python-docx.

Exact package requirements are listed in `requirements.txt`.

## Reproducibility boundary

The repository documents the analytical code, parameter choices and workflow structure. It does not provide unrestricted reproduction of sensitive interview-level analyses because the underlying qualitative material cannot be publicly redistributed.

## Author

Mingyue Zhang  
MSc Data Science dissertation  
Durham University
