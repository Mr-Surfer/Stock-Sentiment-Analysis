# 📈 Stock Sentiment Analysis using Machine Learning

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-NLP-orange)
![Status](https://img.shields.io/badge/Project-Completed-green)

**Author:** Kunal Singh  
**Enrollment No:** 22324025  
**Program:** BS-MS Physics  

---

# 📌 Project Description

Financial markets are heavily influenced by news and public sentiment.  
This project uses **Natural Language Processing (NLP)** and **Machine Learning** to analyze financial news headlines and determine the sentiment associated with them.

The objective is to classify news headlines as **positive, negative, or neutral** and explore how sentiment may reflect investor behavior and potential market trends.

The analysis focuses on two companies:

- Tesla
- Meta

---

# 🎯 Objectives

- Collect financial news headlines
- Perform sentiment analysis on textual data
- Convert text data into numerical features
- Train machine learning models
- Evaluate models using standard metrics
- Compare performance across different algorithms

---

# 🔄 Project Workflow

```
Financial News Headlines
        │
        ▼
Dataset Collection (FINVIZ)
        │
        ▼
Sentiment Analysis (VADER)
        │
        ▼
Dataset Labeling
        │
        ▼
Text Vectorization
        │
        ▼
Machine Learning Models
        │
        ▼
Model Evaluation
        │
        ▼
Performance Comparison
```

---

# 📊 Dataset

The dataset consists of financial news headlines extracted from **FINVIZ**, a financial news aggregation platform.

FINVIZ compiles headlines from multiple financial sources, providing a consistent dataset for sentiment analysis.

Due to restrictions on automated scraping, HTML files were downloaded and parsed locally to extract the headlines.

Separate datasets were prepared for:

- Tesla
- Meta

---

# 💬 Sentiment Analysis

Sentiment analysis was performed using **VADER (Valence Aware Dictionary and Sentiment Reasoner)** from the **NLTK library**.

VADER is designed for analyzing sentiment in short text such as:

- News headlines
- Social media posts
- Reviews

### Custom Financial Lexicon

To improve sentiment detection for financial contexts, additional words were added to the VADER lexicon:

```python
new_words = {
    'crushes': 10,
    'beats': 5,
    'misses': -5,
    'trouble': -10,
    'falls': -100
}
```

These words help better capture sentiment expressed in financial headlines.

---

# 📉 Financial Metrics

Several trading metrics were used to evaluate performance:

### Sharpe Ratio
Measures the **risk-adjusted return** of an investment strategy.

### Maximum Drawdown
Represents the **largest drop from peak to trough** during the trading period.

### Number of Trades
Total number of buy and sell transactions executed.

### Win Ratio
Percentage of profitable trades among the total trades.

---

# 🔤 Text Vectorization

Before training machine learning models, headlines were converted into numerical vectors.

The process included:

- Tokenization
- Text preprocessing
- Feature vector generation
- Dataset preparation for supervised learning

Separate datasets were created for Tesla and Meta.

---

# 🧠 Models Used

The following machine learning models were evaluated:

- Neural Network
- Logistic Regression
- Support Vector Classifier
- Random Forest
- Gradient Boosting
- K-Nearest Neighbors
- Decision Tree

---

# 📊 Results (Tesla Dataset)

| Model | Accuracy | Precision | Recall | F1 Score |
|------|------|------|------|------|
| Neural Network | 0.60 | 0.7056 | 0.60 | 0.5242 |
| Logistic Regression | 43.33% | 42.44% | 43.33% | 41.80% |
| Support Vector Classifier | 46.67% | 75.11% | 46.67% | 29.70% |
| Random Forest | 48.33% | 49.82% | 48.33% | 43.81% |
| Gradient Boosting | 48.33% | 47.28% | 48.33% | 45.23% |
| KNN | 51.67% | 52.04% | 51.67% | 48.93% |
| Decision Tree | 40.00% | 40.53% | 40.00% | 40.10% |

---

# 📊 Results (Meta Dataset)

| Model | Accuracy | Precision | Recall | F1 Score |
|------|------|------|------|------|
| Neural Network | 0.60 | 0.7056 | 0.60 | 0.5242 |
| Logistic Regression | 43.33% | 42.44% | 43.33% | 41.80% |
| Support Vector Classifier | 46.67% | 75.11% | 46.67% | 29.70% |
| Random Forest | 46.67% | 46.67% | 46.67% | 39.85% |
| Gradient Boosting | 48.33% | 47.28% | 48.33% | 45.23% |
| KNN | 51.67% | 52.04% | 51.67% | 48.93% |
| Decision Tree | 40.00% | 39.75% | 40.00% | 39.82% |

---

# 🏆 Best Model

The best performing model after hyperparameter tuning was:

**Support Vector Classifier**

Parameters:

```
C = 1
gamma = 1
kernel = rbf
```

---

# 🛠 Technologies Used

- Python
- NLTK
- VADER Sentiment Analyzer
- Scikit-learn
- Neural Networks
- NumPy
- Pandas
- Matplotlib

---

# 📁 Project Structure

```
Stock-Sentiment-Analysis
│
├── data
│
├── notebooks
│
├── models
│
├── plots
│
├── report
│
└── README.md
```

---

# 🚀 Future Improvements

Possible future improvements include:

- Using **Transformer-based models (BERT / FinBERT)**
- Expanding dataset size
- Integrating real-time financial news APIs
- Applying deep learning models such as **LSTM**
- Developing an automated trading system

---

# 📬 Contact

**Kunal Singh**  
BS-MS Physics  

If you find this project useful, feel free to ⭐ the repository.
