# Product Recommendation System (Embedding-Based)

This project implements a semantic product recommendation system using transformer-based embeddings.  
Given a natural language product query, the system retrieves similar products based on cosine similarity in embedding space.

## Problem
Traditional keyword-based search fails to capture user intent and semantic meaning.  
This system demonstrates how embedding-based retrieval improves relevance and discovery in e-commerce.

## Approach
- Data cleaning and text normalization
- Feature construction via combined product metadata
- Embedding generation using:
  - BERT
  - Sentence Transformers (`all-mpnet-base-v2`)
- Cosine similarity–based retrieval
- Ranking and evaluation against actual purchase data

## Key Techniques
- NLP feature engineering
- Transformer embeddings
- Similarity search
- Ranking evaluation
- Visualization of recommendation success

## Results
- Demonstrates improved semantic relevance compared to keyword matching
- Accurately retrieves purchased items within top-K recommendations
- Scales efficiently with precomputed embeddings

## Notes on Data
Raw datasets are not included due to size and sensitivity.  
Notebook includes clear schema expectations and can be adapted to new datasets.

## Technologies
Python, pandas, NumPy, scikit-learn, Hugging Face Transformers, Sentence Transformers

