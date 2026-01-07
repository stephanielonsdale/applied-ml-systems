# Address Classification with Machine Learning

An **end-to-end applied machine learning pipeline** for classifying noisy address strings into predefined categories.  
This notebook compares a **rule-based (regex) baseline** against a **supervised ML model**, demonstrating how machine learning improves accuracy, scalability, and robustness for real-world text classification tasks.

---

## Overview

Address data in production systems is often noisy, inconsistent, and difficult to parse reliably with rules alone.  
This project demonstrates how a supervised ML approach can outperform a regex-based baseline when classifying address strings at scale.

The notebook walks through the **full ML lifecycle**, from baseline construction to model evaluation and error analysis.

---

## Problem Statement

**Goal:**  
Classify free-form address strings into standardized categories for downstream processing.

**Challenges addressed:**
- Inconsistent formatting
- Abbreviations and typos
- Mixed-use addresses
- Scalability limitations of rule-based systems

---

## Approach

1. **Regex-Based Baseline**
   - Define pattern-based rules for address categorization
   - Establish a transparent but brittle baseline
   - Measure initial performance

2. **Supervised Machine Learning Model**
   - Convert address text into numerical features using `CountVectorizer`
   - Train a supervised classifier on labeled address data
   - Compare performance directly against the regex approach

3. **Evaluation and Analysis**
   - Quantitative metrics (accuracy, precision, recall, F1)
   - Confusion matrices and visualizations
   - Error analysis to identify failure modes and improvement opportunities

---

## What This Notebook Demonstrates

- Baseline vs ML model comparison
- Feature engineering for text data
- Supervised model training and validation
- Metric-driven evaluation
- Practical error analysis
- Visualization of model performance
- Improvement over rule-based systems in real-world data settings

---

## Dataset Notes

- The full training and test datasets are **not included** due to size and sensitivity.
- The notebook expects CSV files with the following schema:

```text
address   (string)
category  (label for training data)
```

- Sample data or schema documentation can be found in the repository’s `data/` directory.

---

## Evaluation Metrics

The following metrics are used to assess performance:

- **Accuracy** – Overall correctness
- **Precision** – Correctness of predicted categories
- **Recall** – Coverage of true categories
- **F1-score** – Balance between precision and recall
- **Confusion Matrix** – Error distribution across classes

Results show a **clear improvement** of the ML model over the regex baseline.

---

## Key Insights

- Regex rules provide transparency but struggle with edge cases
- ML models generalize better to unseen address formats
- Feature-based text models scale more effectively with data volume
- Error analysis reveals concrete opportunities for further improvement

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- Jupyter Notebook
- Matplotlib / Seaborn (visualization)

---

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open the notebook:
   ```bash
   jupyter notebook notebooks/address_classification.ipynb
   ```

3. Provide training and test CSV files matching the expected schema.

---

## Design Philosophy

- **Baseline-first modeling** to quantify improvement
- **Evaluation-driven iteration**
- **Readable, explainable pipelines**
- **Production-aware ML practices**

---

## Author

**Stephanie Lonsdale**  
Graduate Student, AI Engineering  
Johns Hopkins University
