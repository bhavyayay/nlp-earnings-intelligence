# 🧾 Earnings Intelligence — NLP Analysis of Earnings Calls & Market Reaction

### **Overview**

Earnings calls contain valuable signals about future company performance.
This project builds an **NLP-powered financial intelligence pipeline** that processes earnings call transcripts, extracts linguistic sentiment, identifies key topics, and correlates them with subsequent price movement.

The goal is to answer a predictive question:

> **Does management language influence short-term market reaction?**

---

## 🧰 **Tech Stack**

* **Python**
* NLP: `NLTK`, `spaCy`, `regex`, TF-IDF
* Topic Modeling: **LDA**
* ML Modeling: **Logistic Regression**
* Visualization: `Matplotlib`, `Seaborn`
* Data: `Earnings Call Transcripts`, `S&P 100`

---

## 📂 **Project Structure**

```
nlp-earnings-intelligence
│
├── data/                          # price & transcript data
├── notebooks/
│   ├── 01_preprocessing.ipynb     # cleaning + tokenization
│   ├── 02_topic_modeling.ipynb    # LDA analysis
│   └── 03_sentiment_model.ipynb   # logistic regression model
├── models/
│   └── processed_outputs.json
├── visualizations/
│   └── lda_topics.png
└── README.md
```

(*Note: folder names reflected in cleaned repo*)

---

## 🧠 **NLP Pipeline**

✔ **1. Preprocessing**

* lowercasing
* stopword removal
* stemming + lemmatization
* tokenization

✔ **2. Feature Extraction**

* TF-IDF vectorization for semantic encoding

✔ **3. Topic Modeling (LDA)**
Extracts latent themes such as:

* pricing strategy
* revenue guidance
* risk exposure
* macroeconomic commentary

✔ **4. Sentiment Classification**
Models management sentiment using:

> **Positive vs Negative Tone → Price Movement**

---

## 📈 **Results**

* Language sentiment is weakly predictive of short-term movement
* Management tone correlated with:

  * bullish earnings pop
  * downward guidance corrections
* Topic categories predicted volatility spikes

(*future work will validate across more companies*)

---

## 🚀 **Future Enhancements**

Planned improvements:

* integrate **deep transformer models** (BERT/FinBERT)
* add **RNN time-series correlation**
* improve labeling using event windows
* deploy to web (Streamlit dashboard)
* ingest more tickers & quarters

---

## 🔧 **Setup & Reproduction**

Clone repository:

```bash
git clone https://github.com/bhavyayay/nlp-earnings-intelligence
cd nlp-earnings-intelligence
pip install -r requirements.txt
```

---

## 🎯 **Applications**

* quant research
* trading intelligence
* investor sentiment analysis
* financial NLP benchmarking

---

## 👤 **Author**

Developed by **Bhavya**

---
