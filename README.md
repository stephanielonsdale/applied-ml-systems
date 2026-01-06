# Applied ML Systems Portfolio 
End-to-end machine learning pipelines built in Python for real-world datasets, including: 
- Address classification (15k+ labeled records)
- Product recommendation system

## Highlights 
- Full ML workflow: preprocessing → feature engineering → training → evaluation
- Model comparison and validation
- Iterative tuning (hyperparameters, feature set adjustments)

## Projects

### 1) Address Classification
**Goal:** Classify noisy address strings into standardized categories for downstream processing.

**Approach:**
- Cleaning + normalization
- Feature engineering
- Supervised classification
- Error review on misclassified samples

**Evaluation:**
- Accuracy + precision/recall
- Cross-validation

### 2) Product Recommendation System 
**Goal:** Recommend relevant products based on user/item signals.

**Approach:**
- Data preprocessing and feature construction
- Baseline vs improved model comparison
- Evaluation and iteration
  
## Tech Stack
Python, pandas, NumPy, scikit-learn, Jupyter 

## Repo Structure
- `notebooks/` – experiments and analysis
- `src/` – reusable functions (preprocessing, training, evaluation)
- `data/sample/` – small sample datasets (no raw data committed)

## How to Run
1. Create env and install dependencies: `pip install -r requirements.txt`
2. Open notebooks in `notebooks/`

## Notes
Raw datasets are not included in this repo; see `data/README.md` for expected schema.
