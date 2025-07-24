# Vector Space Model for Information Retrieval
This project implements and compares several Information Retrieval (IR) models using the Vector Space Model (VSM) on the Cranfield dataset.

## Models Implemented
1. Weighting Schemes: TF-IDF, Okapi BM25, and Log-Entropy.
2. Semantic Analysis: Latent Semantic Analysis (LSA) using Truncated SVD for dimensionality reduction.
   
Evaluation: Performance is measured using Precision@10, Recall@10, and MAP@10.

## Architecture
<img width="293" height="367" alt="vsm_architecture" src="https://github.com/user-attachments/assets/80a03857-5997-4657-8348-5187dcacefc6" />

## Results
- Best Standalone Model: BM25 was the top performer on its own (MAP@10=0.6944).
- Best Semantic Model: Log-Entropy + LSA achieved the highest performance among LSA-enhanced models (MAP@10≈0.693).
- LSA is Not Always Better: Adding LSA can sometimes degrade the performance of strong baseline models like BM25.

## Tech Stack
- Python
- scikit-learn: For TF-IDF, TruncatedSVD (LSA), and cosine similarity.
- spaCy: For efficient tokenization and lemmatization.
- NLTK: For its English stopword list.
- pandas & NumPy: For data manipulation and numerical operations.

