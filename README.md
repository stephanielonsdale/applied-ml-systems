# Applied Machine Learning Systems Portfolio

A collection of **end-to-end applied machine learning pipelines** built in Python on real-world datasets.  
This repository emphasizes **clean data workflows, model evaluation, and iterative improvement**, reflecting how ML systems are developed in practice.

---

## Overview

This portfolio showcases applied ML projects that span the full lifecycle:

**data preprocessing → feature engineering → model training → evaluation → iteration**

The focus is on **practical system-building**, not just model fitting, with attention to data quality, validation, and error analysis.

---

## Highlights

- Full supervised ML workflows from raw data to evaluated models  
- Feature engineering and normalization for noisy, real-world inputs  
- Model comparison and validation strategies  
- Iterative tuning (hyperparameters, feature sets, error-driven refinement)  
- Emphasis on interpretability and performance trade-offs  

---

## Projects

### 1) Address Classification

**Goal:**  
Classify noisy address strings into standardized categories for downstream processing and analytics.

**Dataset:**  
15k+ labeled address records with real-world inconsistencies.

**Approach:**
- Data cleaning and normalization
- Feature engineering (string-based and structural features)
- Supervised classification
- Error analysis on misclassified samples

**Evaluation:**
- Accuracy
- Precision / Recall
- Cross-validation

---

### 2) Product Recommendation System

**Goal:**  
Recommend relevant products based on user and item interaction signals.

**Approach:**
- Data preprocessing and feature construction
- Baseline vs improved model comparison
- Iterative evaluation and refinement

**Evaluation:**
- Offline performance metrics
- Comparative model analysis

---

## Tech Stack

- Python
- pandas
- NumPy
- scikit-learn
- Jupyter Notebook

---

## Repository Structure

```text
applied-ml-systems/
├── notebooks/        # Experiments and analysis notebooks
├── src/              # Reusable ML utilities (preprocessing, training, evaluation)
├── data/
│   └── sample/       # Small sample datasets (no raw data committed)
├── README.md
└── requirements.txt
```

---

## How to Run

1. Create an environment and install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open and run notebooks:
   ```bash
   jupyter notebook notebooks/
   ```

---

## Notes

- Raw datasets are **not included** in this repository.
- See `data/README.md` for expected schemas and data formats.
- Projects are designed to be **reproducible** using provided sample data.

---

## Design Philosophy

- **Data quality first** — preprocessing and validation matter as much as modeling  
- **Evaluation-driven development** — metrics guide iteration  
- **Clarity over complexity** — readable pipelines over opaque solutions  
- **Production-aware mindset** — systems reflect real deployment considerations  

---

## Author

**Stephanie Lonsdale**  
Graduate Student, AI Engineering  
Johns Hopkins University
