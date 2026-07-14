# 🧬 COPD Microbiome Explorer

An interactive Streamlit dashboard for end-to-end analysis and visualization of 16S rRNA microbiome sequencing data from COPD and Healthy individuals.

**Live App:** https://copd-microbiome-dashboard-krupalipoharkar.streamlit.app/

---

## Overview

This project demonstrates a complete microbiome bioinformatics workflow starting from raw sequencing data through quality control, taxonomic profiling, diversity analysis, statistical testing, machine learning, and explainable AI.

The dashboard allows users to interactively explore sequencing quality, microbial composition, diversity metrics, predictive machine learning models, and model interpretability.

---

## Objectives

- Compare sputum microbiomes between COPD and Healthy individuals
- Identify microbial genera associated with COPD
- Evaluate machine learning models for disease classification
- Interpret model predictions using Explainable AI (SHAP and LIME)
- Provide an interactive visualization platform for microbiome research

---

## Bioinformatics Workflow

```
Raw FASTQ
      ↓
FastQC & MultiQC
      ↓
QIIME2 Import
      ↓
DADA2 Denoising
      ↓
ASV Generation
      ↓
SILVA Taxonomic Assignment
      ↓
Alpha Diversity
      ↓
Beta Diversity
      ↓
Relative Abundance Analysis
      ↓
Machine Learning
      ↓
SHAP & LIME Explainability
      ↓
Interactive Streamlit Dashboard
```

---

## Technologies Used

### Bioinformatics

- QIIME2
- DADA2
- SILVA Database

### Data Analysis

- Python
- Pandas
- NumPy
- SciPy

### Machine Learning

- Random Forest
- Logistic Regression
- Gradient Boosting
- XGBoost

### Explainable AI

- SHAP
- LIME

### Visualization

- Matplotlib
- Plotly
- Streamlit

---

## Dashboard Features

### 🏠 Overview
Project summary and analysis workflow.

### 🧪 Quality Control
- FastQC reports
- MultiQC summaries

### 🦠 Taxonomy
- Relative abundance
- Taxonomic composition
- Genus distribution

### 🧬 Diversity
- Alpha diversity
- Beta diversity
- PCoA visualization
- Statistical comparisons

### 🔬 ASV Explorer
Interactive exploration of ASV abundance tables.

### 🤖 Machine Learning
Performance comparison of multiple classification models including:

- Random Forest
- Logistic Regression
- Gradient Boosting
- XGBoost

with:

- ROC Curves
- Confusion Matrices
- Feature Importance

### 🔍 SHAP
Global and local explanation of XGBoost predictions including:

- SHAP Beeswarm
- SHAP Bar Plot
- Waterfall Plot

### 💡 LIME
Sample-level explanation of model predictions.

### 🎯 Serratia Analysis
Detailed exploration of Serratia abundance and its contribution to COPD classification.

### ⚠ Limitations
Study limitations and interpretation notes.

---

## Machine Learning Models

The following supervised learning algorithms were evaluated:

| Model | Purpose |
|--------|----------|
| Random Forest | Tree ensemble classifier |
| Logistic Regression | Linear baseline model |
| Gradient Boosting | Boosted decision trees |
| XGBoost | Optimized gradient boosting |

Performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Cross-validation

---

## Explainable AI

The project incorporates Explainable AI techniques to improve biological interpretation.

### SHAP

Provides:

- Global feature importance
- Sample-level explanations
- Feature contribution analysis

### LIME

Provides:

- Local interpretation for individual predictions
- Feature contribution visualization

---

## Dataset

The microbiome dataset contains genus-level relative abundance profiles from sputum samples of:

- COPD patients
- Healthy controls

The workflow follows standard 16S rRNA microbiome analysis practices using QIIME2 and DADA2.

---

## Repository Structure

```
app.py
requirements.txt

data/
figures/
models/

results/

README.md
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/krupali23/copd-microbiome-explorer.git
```

Move into the project

```bash
cd copd-microbiome-explorer
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the dashboard

```bash
streamlit run app.py
```

---

## Author

**Dr. Krupali Poharkar**

PhD Biotechnology (Microbiology)

Bioinformatics | Microbiome | Machine Learning | Explainable AI | Single-cell RNA-seq | NGS Analysis

GitHub:
https://github.com/krupali23

LinkedIn:
https://www.linkedin.com/in/krupalipoharkar/

---

## Citation

If you find this project useful for your research, please consider citing or referencing this repository.

---

## License

This project is intended for educational and research purposes.
