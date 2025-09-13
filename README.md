# 955-dissertation
** Natural Language Processing and Customer Insight Development from Product Reviews**
This repository contains the code and experiments for my MSc dissertation

## Clone the repo:
check the code from :git clone https://github.com/Matthewaxe123/955-dissertation.git
cd 955-dissertation
It implements an end-to-end NLP pipeline on large-scale e-commerce reviews:

- **EDA** – length distributions, stopwords, punctuation, bigrams  
- **Topic Modelling** – LDA vs. BERTopic  
- **Sentiment Classification** – TF-IDF ML (SVM, Naive Bayes, Logistic Regression), VADER, and fine-tuned BERT  
- **Extractive Summarisation** – LexRank (continuous/thresholded graphs) with MMR

The goal is not to propose a new algorithm, but to compare methods side-by-side under a consistent framework and give practical guidance for real-world use.


## Dataset
- **Source:** Amazon Review Polarity (Zhang, 2015)  
The original dataset is held by the project supervisor and is **not redistributed** due to size and licensing constraints.
## How to request acess (examiners only)
Supervisor Email:<Martyn.Parker@warwick.ac.uk>
- **Size:** 3.6M training reviews, 0.4M test reviews  
- **Labels:** `1 = Negative`, `2 = Positive`  
- **Usage in this project:** balanced random subsets per split  
  (1,000 negative + 1,000 positive, fixed seed) for tractable experiments

## Requirements:
- **Python:** 3.11.x 
Create a virtual environment in this directory (must have python3 already installed on the computer)
All packages and libraries are shown in <https://github.com/Matthewaxe123/955-dissertation.git>
### Install (macOS/Linux)
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
Method:Topic Modelling

LDA (Latent Dirichlet Allocation)

BERTopic (transformer-based embeddings + clustering)

Evaluation: C_V Coherence, interpretability, visualization.

Sentiment Analysis

Traditional ML: SVM, Naive Bayes, Logistic Regression (TF-IDF features).

Lexicon-based: VADER.

Transformer-based: Fine-tuned BERT.

Hybrid: VADER + BERT ensemble.

Evaluation: Accuracy, Precision, Recall, F1-score + confusion matrices


### Contributors
·  Main contributor: Yu Ma

·  Supervisor: Dr Martyn Parker


