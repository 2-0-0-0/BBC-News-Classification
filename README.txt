 🧠 News Category Classification using LSTM & BiLSTM

This repository presents a complete text classification pipeline for BBC News Articles, moving from classical machine learning baselines to advanced deep learning models like LSTM and Bidirectional LSTM (BiLSTM). Along the way, we explore data cleaning, EDA, feature engineering, model tuning, and performance visualization — all within a reproducible and modular codebase.

 📌 Problem Statement

Predict the category (e.g., tech, sport, business) of a given news article using natural language processing (NLP) techniques and supervised machine learning.

🔍 Dataset

- Source: BBC News Articles Dataset
- Attributes:
  - `text`: The full news article
  - `category`: One of the target categories (e.g., business, entertainment, politics, sport, tech)

🧹 Preprocessing Pipeline

- Lowercasing and punctuation removal
- Stopword elimination
- Tokenization and lemmatization
- TF-IDF vectorization (for classical models)
- Tokenizer + padded sequences (for LSTM models)
- Label encoding of categories

 📊 Exploratory Data Analysis

- Distribution of news categories
- Top words across and within categories
- Word frequency bar plots
- Category-specific word clouds

 🤖 Models Implemented

 Classical Machine Learning

| Model                     | Vectorization | Accuracy |
|--------------------------|---------------|----------|
| Logistic Regression      | TF-IDF        | 88.7%    |
| Multinomial Naive Bayes  | TF-IDF        | 86.9%    |
| Linear SVM               | TF-IDF        | 89.3%    |
| Random Forest            | TF-IDF        | 83.5%    |

Deep Learning

 LSTM

- Embedding size: 128
- LSTM layer: 100 units
- Dropout (0.3) for regularization
- Result: Test Accuracy ~90.56%

 Bidirectional LSTM

- BiLSTM Layer: 100 units
- Dropout regularization
- Result: Improved Test Accuracy (e.g., ≥91%)

📈 Visualizations

- Accuracy & loss across epochs
- Side-by-side comparison of LSTM vs BiLSTM
- Misclassified sample analysis
- Confusion matrix

## 🔁 Model Flow

Dataset → Cleaning → Label Encoding → Vectorization ↘ ↙ Classical Models LSTM / BiLSTM ↓ ↓ Evaluation Fine-Tuning & Visuals



