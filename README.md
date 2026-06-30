# Geometrik Retorik (Geometric Rhetoric)

**Exploratory analysis of U.S. presidential rhetoric using Moral Foundations Theory, Principal Component Analysis (PCA), and dynamic speech analysis.**

---

## Overview

This repository contains the source code, processed datasets, and analysis used in the study:

> **Büyük Toplumun Ahlaki Salınım Eksenleri**
>
> *An exploratory study on United States presidential speeches (1789–2020).*

The project investigates whether political leaders share common rhetorical structures despite speaking in different historical periods.

Instead of treating speeches as collections of words, the study represents them as trajectories in a five-dimensional moral space derived from **Moral Foundations Theory (MFT)**.

---

## Research Question

Can centuries of political speeches be explained by a small number of common moral-rhetorical dimensions?

To investigate this question, every available U.S. presidential speech between **1789 and 2020** was analyzed using:

- Moral Foundations Theory (MFT)
- eMFDscore
- Principal Component Analysis (PCA)
- Dynamic projection analysis
- Time-series analysis of speeches

---

## Main Contributions

- Construction of a five-dimensional moral embedding of presidential rhetoric.
- PCA analysis of the entire historical corpus.
- Interpretation of the five principal rhetorical axes.
- Dynamic sentence-by-sentence projection of speeches onto PCA space.
- Exploration of recurring rhetorical structures across different presidents and historical periods.

---

## Dataset

The original presidential corpus used in this project was obtained from the **American Presidency Project** (University of California, Santa Barbara), which provides public access to United States presidential documents.

The JSON version of the corpus (`presidency.json`) was downloaded from Kaggle and subsequently processed for this research.

Original data source:
- The American Presidency Project (University of California, Santa Barbara)
  https://www.presidency.ucsb.edu/

Kaggle dataset:
- https://www.kaggle.com/
  (https://www.kaggle.com/datasets/jayrav13/american-presidency-project)

The processed datasets included in this repository were generated as part of this project.

Coverage:

- 1789–2020
- Presidential speeches
- Inaugural addresses
- Executive messages
- Radio and television speeches
- International speeches
- Debates
- Party platforms

---

## Repository Structure

```
processed_corpus/      Processed datasets
selected_speeches/     Speech-level analysis
pca_export/            PCA outputs
analysis/              Analysis notebooks and scripts
plots/                 Figures and visualizations
```

---

## Technologies

- Python
- pandas
- NumPy
- scikit-learn
- Plotly
- eMFDscore

---

## Data Processing Pipeline

American Presidency Project
          ↓
      Kaggle JSON
          ↓
Cleaning
          ↓
Sentence segmentation
          ↓
eMFDscore
          ↓
PCA
          ↓
Dynamic projection analysis
          ↓
Figures & paper

---
## Paper

The complete paper is included in this pdf file.

**Title**

> Büyük Toplumun Ahlaki Salınım Eksenleri

---

## Citation

If you use this repository or build upon this work, please cite:

```
Yiğit Ozan Berk.
Büyük Toplumun Ahlaki Salınım Eksenleri.
Istanbul, Turkiye - 2026.
```

---

## License

This project is released under the MIT License.
You are free to use, modify, and distribute this software under the terms of the license.

---

## Author

**Yiğit Ozan Berk**

Istanbul, Türkiye

GitHub:
https://github.com/yigitozanberk


Third-Party Software Notice

This repository contains original research, source code, documentation, and analysis developed by the author.

Some analyses in this project were generated using the eMFDscore library for Moral Foundations Dictionary (eMFD) feature extraction. The eMFDscore software is not included in this repository and remains subject to its own license terms.

Users wishing to reproduce the complete analysis pipeline should obtain and install eMFDscore separately and comply with its licensing requirements.

This repository does not redistribute or modify the eMFDscore source code. All original code contained in this repository is released under the MIT License unless otherwise stated.
