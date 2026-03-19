# NLP Research Analyzer

An end-to-end Natural Language Processing (NLP) system for analyzing, comparing, and extracting insights from research documents using both lexical (TF-IDF) and semantic (Sentence-BERT) representations.

---

## Overview

The NLP Research Analyzer is designed to process and analyze multiple research documents through a unified pipeline. It integrates classical NLP techniques with modern embedding-based approaches to enable similarity analysis, clustering, topic modeling, and summarization.

The system emphasizes comparative evaluation between lexical and contextual representations to demonstrate the effectiveness of modern NLP methods.

---

## Key Features

* Document similarity analysis using TF-IDF and Sentence-BERT
* Clustering of documents with dimensionality reduction (PCA / TruncatedSVD)
* Topic modeling using Latent Dirichlet Allocation (LDA)
* Extractive text summarization
* Interactive visualizations for similarity and clustering
* Streamlit-based interface for real-time analysis

---

## Technical Stack

**Language**

* Python

**Core Libraries**

* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

**NLP & Embeddings**

* NLTK
* Sentence-Transformers (SBERT)

**Visualization**

* Plotly

**Application Layer**

* Streamlit

---

## System Architecture

The system follows a modular pipeline:

1. **Preprocessing Layer**

   * Text cleaning, tokenization, stopword removal, and lemmatization

2. **Representation Layer**

   * TF-IDF (sparse lexical representation)
   * Sentence-BERT (dense semantic embeddings)

3. **Analysis Layer**

   * Similarity computation
   * K-Means clustering
   * Topic modeling (LDA)
   * Extractive summarization

4. **Dimensionality Reduction**

   * PCA / TruncatedSVD for visualization

5. **Visualization Layer**

   * Cluster plots
   * Similarity matrices
   * Interactive dashboards

---

## Evaluation

The system evaluates the effectiveness of lexical versus semantic representations for document clustering.

* Semantic embeddings (SBERT) demonstrated improved clustering coherence
* Higher silhouette scores observed for semantic representations
* Results highlight the limitations of purely lexical approaches in capturing contextual meaning

---

## Usage

### Installation

```bash
git clone https://github.com/KaavyaGala546/NLP_Research_Analyser.git
cd NLP_Research_Analyser

pip install -r requirements.txt
```

### Run Application

```bash
streamlit run app.py
```

---

## Project Structure

```
NLP_Research_Analyser/
│
├── app.py                # Streamlit application entry point
├── preprocessing.py     # Text preprocessing pipeline
├── modeling.py          # Vectorization, clustering, and topic modeling
├── utils.py             # Utility functions
├── create_corpus.py     # Dataset preparation
├── requirements.txt     # Dependencies
├── report.tex           # Research documentation (LaTeX)
└── workflows/           # Processing workflows
```

---

## Limitations

* Designed for structured research-style documents
* Unsupervised evaluation metrics depend on dataset characteristics
* Performance may vary with corpus size and diversity

---

## Future Work

* Integration of transformer-based abstractive summarization
* Optimization for large-scale datasets
* Deployment as a scalable web application
* Enhanced user interface and interaction design

---

## Author

Kaavya Gala

---

## Notes

This project was developed to explore practical NLP system design and evaluate the performance differences between classical vectorization techniques and modern embedding-based approaches.
