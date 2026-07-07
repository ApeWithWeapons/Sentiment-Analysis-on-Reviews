# Sentiment Analysis on Amazon Reviews

NLP project classifying Amazon product reviews as positive or negative 
using a sample of 200,000 reviews from a dataset of 3.6 million.

## Project Overview
I built and compared three text classification models using TF-IDF 
vectorisation to convert raw review text into numeric features. This 
is my first project working with unstructured text data, introducing 
text preprocessing, TF-IDF, and NLP-specific model selection.

## Key Findings

| # | Theme | Finding |
|---|-------|---------|
| 1 | Balance | Dataset was nearly perfectly balanced — 50/50 positive/negative split |
| 2 | Review Length | Negative reviews are slightly longer — unhappy customers write more |
| 3 | Best Model | LinearSVC achieved the highest accuracy on the TF-IDF matrix |
| 4 | Interpretability | Logistic Regression coefficients reveal which words most strongly predict each sentiment |
| 5 | Speed | Naive Bayes trained fastest while remaining competitive in accuracy |

## Models Compared
- **Logistic Regression** — interpretable baseline, strong NLP performer
- **Multinomial Naive Bayes** — probabilistic model designed for text, fastest to train
- **LinearSVC** — best accuracy, optimised for large sparse matrices

## Tools Used
Python, pandas, numpy, matplotlib, seaborn, scikit-learn, re

## Dataset
[Amazon Reviews — Kaggle](https://www.kaggle.com/datasets/bittlingmayer/amazonreviews)
