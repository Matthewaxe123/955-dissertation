# 955-dissertation
This repository contains the code and experiments for my MSc dissertation:
"Natural Language Processing and Customer Insight Development from Product Reviews" 

ST955_dissertation_U1997397 (9)
The project builds an end-to-end NLP pipeline to extract insights from large-scale e-commerce reviews. Using the Amazon Review Polarity dataset, the pipeline integrates:

Exploratory Data Analysis (EDA) – length distributions, stopwords, punctuation, bigram analysis.

Topic Modelling – comparison of LDA and BERTopic.

Sentiment Classification – traditional ML (SVM, Naive Bayes, Logistic Regression), VADER, and fine-tuned BERT.

Extractive Summarisation – LexRank with continuous/thresholded graphs and MMR.

The aim is not to propose a new algorithm, but to compare methods side-by-side under a consistent framework and provide practical guidance on which methods work best in real-world applications

Source: Amazon Review Polarity dataset (Zhang, 2015)

Size: 3.6M training reviews, 0.4M test reviews.

Labels:

1 = Negative

2 = Positive

Usage in this project: Balanced subsets (1,000 negative + 1,000 positive per split, fixed seed) for tractable experiments

ST955_dissertation_U1997397 (9)

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

ST955_dissertation_U1997397 (9)
Summarisation

LexRank (continuous & thresholded)

MMR (λ=0.7) with word-budget ≈110 words.

Outputs: concise summaries highlighting consensus in each subset.

check the code from :git clone https://github.com/Matthewaxe123/955-dissertation.git
cd 955-dissertation
