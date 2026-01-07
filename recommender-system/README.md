# Product Recommendation System (Embedding-Based)

An **embedding-based semantic product recommendation system** built using transformer models.  
Given a natural language product query, the system retrieves semantically similar products using **cosine similarity in embedding space**, demonstrating how modern NLP improves relevance over traditional keyword search.

---

## Overview

Traditional keyword-based search struggles to capture **user intent**, semantic similarity, and nuanced product descriptions.  
This project demonstrates how **transformer-based embeddings** enable more accurate product discovery by representing items in a shared semantic vector space.

The notebook implements an end-to-end recommendation pipeline, from data preprocessing to embedding generation, retrieval, evaluation, and visualization.

---

## Problem Statement

**Goal:**  
Recommend relevant products based on semantic similarity rather than keyword overlap.

**Challenges addressed:**
- Vocabulary mismatch between queries and product descriptions
- Poor recall in keyword-based systems
- Scalability for large product catalogs
- Ranking relevance based on semantic meaning

---

## Approach

1. **Data Cleaning and Normalization**
   - Remove duplicates and missing values
   - Normalize text (lowercasing, character filtering)
   - Combine multiple product metadata fields into a single text representation

2. **Feature Construction**
   - Concatenate product name, category, and description into a unified text field
   - Prepare text for embedding-based similarity comparison

3. **Embedding Generation**
   - Baseline embeddings using **BERT**
   - Improved embeddings using **Sentence Transformers (`all-mpnet-base-v2`)**
   - Precompute embeddings for efficient retrieval

4. **Similarity-Based Retrieval**
   - Compute cosine similarity between query embeddings and product embeddings
   - Rank products by similarity score
   - Retrieve top-K recommendations

5. **Evaluation Against Purchase Data**
   - Validate recommendations using real purchase records
   - Measure whether purchased items appear in top-K results
   - Analyze ranking positions and failure cases

---

## What This Notebook Demonstrates

- Embedding-based semantic search
- Comparison between BERT and Sentence Transformer embeddings
- Scalable similarity search using precomputed vectors
- Ranking evaluation using real user behavior
- Visualization of recommendation success and failure
- Business relevance of semantic retrieval in e-commerce systems

---

## Evaluation Metrics

The system is evaluated using:

- **Top-K accuracy** (whether purchased product appears in recommendations)
- **Purchase rank distribution**
- **Match vs no-match analysis**
- **Qualitative inspection of recommendation relevance**

Results show improved semantic relevance compared to keyword-based approaches.

---

## Dataset Notes

- Raw datasets are **not included** due to size and sensitivity.
- The notebook expects structured CSV files with fields such as:

```text
product_name
product_category
description
```

- A separate purchase dataset is used for evaluation, linking queries to purchased products.

The notebook includes clear schema expectations and can be adapted to new datasets.

---

## Key Techniques Used

- NLP feature engineering
- Transformer-based embeddings
- Sentence Transformers for semantic similarity
- Cosine similarity search
- Ranking evaluation
- Visualization of recommendation performance

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- Hugging Face Transformers
- Sentence Transformers
- Jupyter Notebook
- Matplotlib / Seaborn

---

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open the notebook:
   ```bash
   jupyter notebook notebooks/product_recommendation_embeddings.ipynb
   ```

3. Provide product metadata and purchase datasets matching the expected schema.

---

## Key Insights

- Semantic embeddings outperform keyword matching for product discovery
- Sentence Transformers provide more consistent similarity rankings than raw BERT embeddings
- Precomputed embeddings enable efficient scaling to large catalogs
- Evaluation against real purchase behavior reveals practical system strengths and weaknesses

---

## Design Philosophy

- **Intent over keywords**
- **Evaluation-driven development**
- **Scalability-aware system design**
- **Business-aligned ML decisions**

---

## Author

**Stephanie Lonsdale**  
Graduate Student, AI Engineering  
Johns Hopkins University
