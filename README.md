# 🧬 CMV/EBV TCR Repertoire Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-data%20analysis-lightblue.svg)
![SciPy](https://img.shields.io/badge/SciPy-statistics-orange.svg)
![Matplotlib](https://img.shields.io/badge/visualization-matplotlib-green.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-statistics-blueviolet.svg)
![Status](https://img.shields.io/badge/status-research%20project-brightgreen.svg)

---

## 📌 Overview

This project presents a computational analysis of CMV-associated T-cell receptor (TCR) repertoires using paired α/β chain data. It investigates sequence-level patterns, gene usage, and physicochemical properties of CDR3 regions, with comparison against a human baseline repertoire.

The goal is to distinguish **true antigen-driven signatures** from **background repertoire structure**.

---

## 🎯 Objectives

- Characterize CDR3β motif patterns (e.g., `CASS...F/Y/E`)
- Compare CMV-specific repertoires with a human baseline
- Identify motif enrichment and depletion patterns
- Analyze public vs private clonotypes
- Explore physicochemical properties of CDR3 terminal residues
- Investigate TRBV/TRAV gene–motif associations

---

## 🧪 Methods

### 1. Data Processing
- Source: VDJdb-derived CMV and human baseline datasets  
- Cleaning: sequence filtering and gene normalization  
- Separation of TRA and TRB chains for paired analysis  

---

### 2. Motif Analysis
CDR3β sequences were grouped into:

- `CASS...F`  
- `CASS...Y`  
- `CASS...E`  
- Other  

Metrics:
- Frequency distribution
- Cross-dataset comparison

---

### 3. Enrichment Analysis

log2(CMV frequency / Human frequency)

- Positive values → enrichment in CMV repertoire  
- Negative values → depletion  

---

### 4. Public vs Private Clonotypes

- **Public:** shared across multiple individuals  
- **Private:** unique to a single individual  

---

### 5. Physicochemical Profiling

Terminal amino acids grouped into:

- Aromatic  
- Hydrophobic  
- Positively charged  
- Negatively charged  
- Other  

---

### 6. Statistical Analysis

- Chi-square test for TRBV/TRAV vs motif association  
- Cramér’s V for effect size estimation  

---

## 📊 Key Findings

- `CASS...F` motifs dominate but are not CMV-specific  
- CMV repertoires show enrichment in hydrophobic and charged residues  
- Negative residues show strong relative enrichment  
- Public TCRs are more conserved than private ones  
- TRBV/TRAV usage shows structured motif associations  

---

## 🧠 Interpretation

After baseline normalization, several apparent enrichments were reduced, suggesting that part of the signal reflects intrinsic repertoire structure rather than CMV-specific antigen selection alone.

---

## ⚠️ Limitations

- TRA/TRB pairing depends on dataset annotations  
- Low-frequency categories may inflate enrichment values  
- Motif abstraction simplifies sequence complexity  
- Limited donor diversity control  

---

## 🛠 Tools & Libraries

- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scipy  

---

## 🚀 Future Work

- Position-specific amino acid analysis  
- Diversity and entropy metrics  
- Machine learning models for TCR specificity  
- Cross-virus comparisons (CMV vs EBV)  
- Sequence embedding approaches  

---

## 📂 Repository Structure
