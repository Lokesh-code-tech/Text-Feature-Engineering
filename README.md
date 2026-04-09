# 📊 Text Feature Engineering & Sentiment Analysis

## 🚀 Project Overview

This project focuses on building an end-to-end NLP pipeline for **sentiment analysis** using customer reviews collected from an e-commerce platform.

The workflow includes:

* Web scraping
* Text preprocessing
* Feature engineering (OHE, BoW, TF-IDF)
* Model building using Logistic Regression

---

## 📁 Dataset

* **Source**: Web scraped from an e-commerce website
* **Size**: 758 customer reviews
* **Features**:

  * Review text
  * Product rating

The dataset was stored in a CSV file and processed using pandas.

---

## 🧹 Data Preprocessing

The following steps were applied to clean the text data:

* Convert text to lowercase
* Remove punctuation
* Remove stopwords

This helps in reducing noise and improving model performance.

---

## 📊 Exploratory Analysis

Most frequent words found in reviews:

> **good, quality, sound, battery, product, earbuds**

These keywords highlight the main aspects users focus on while reviewing products.

---

## ⚙️ Feature Engineering

Three techniques were used to convert text into numerical format:

### 1. One-Hot Encoding (OHE)

* Binary representation (0/1)
* Indicates presence of words

### 2. Bag of Words (BoW)

* Counts frequency of words
* Simple and effective baseline

### 3. TF-IDF Vectorization

* Assigns importance to words
* Reduces weight of common words

---

## 🤖 Model Building

* Model used: **Logistic Regression**
* Target variable:

  * Positive → Rating ≥ 3
  * Negative → Rating < 3

---

## 📈 Results

| Method       | Accuracy |
| ------------ | -------- |
| Bag of Words | 0.93     |
| TF-IDF       | 0.90     |

### 🔍 Insights

* BoW slightly outperformed TF-IDF in this dataset
* Both models achieved strong performance

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* NLTK
* BeautifulSoup (for web scraping)

---

## 📌 Key Learnings

* Importance of text preprocessing in NLP
* Difference between BoW and TF-IDF
* Handling sparse data
* Building baseline ML models for text classification

---

## 🔮 Future Improvements

* Use advanced embeddings (Word2Vec, GloVe, BERT)
* Hyperparameter tuning
* Try advanced models (XGBoost, Deep Learning)
* Improve scraping pipeline for larger datasets

---

## 📎 Conclusion

This project demonstrates a complete NLP pipeline from raw text data to model evaluation. It highlights how feature engineering techniques impact model performance and provides a strong foundation for more advanced NLP tasks.

---
