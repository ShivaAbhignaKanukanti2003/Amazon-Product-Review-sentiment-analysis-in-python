# Amazon Product Reviews Sentiment Analysis 🛒📊

An end-to-end **Natural Language Processing (NLP)** project that analyzes Amazon product reviews and classifies customer sentiment as **positive or negative** using **TF-IDF feature extraction** and **Logistic Regression** within a clean, leakage-free machine learning pipeline.

---

## 🚩 Problem Statement

Online reviews strongly influence purchasing decisions. Manually analyzing thousands of customer reviews is time-consuming and subjective.  
This project builds an **automated sentiment analysis system** that converts raw customer reviews into structured insights using classical NLP and machine learning techniques.

---

## 🎯 Project Objectives

- Convert unstructured text reviews into numerical features using NLP
- Classify sentiment as **positive** or **negative**
- Build a clean, production-ready ML pipeline
- Handle missing data and class imbalance correctly
- Evaluate model performance using meaningful metrics

---

## 📊 Dataset Overview

**Amazon Product Reviews Dataset**

- Columns:
  - `Review` – customer review text
  - `Sentiment` – numerical rating (1–5)
- Sentiment Mapping:
  - Rating `> 3` → **Positive (1)**
  - Rating `≤ 3` → **Negative (0)**
- Dataset contains missing values, handled safely during preprocessing

---

## 🔧 Text Preprocessing (NLP)

Minimal and effective preprocessing is applied directly inside the pipeline:

- Lowercasing text
- Removing punctuation and non-alphabetic characters
- Removing English stopwords
- Defensive handling of missing or invalid text entries

This ensures robustness and prevents runtime errors during training.

---

## 🧠 Feature Extraction

### TF-IDF Vectorization
- Converts text into numerical vectors
- Captures importance of words across the corpus
- Uses **unigrams + bigrams** to detect phrases like *“not good”*
- Limits vocabulary size to improve efficiency

---

## 🤖 Model Architecture

### Logistic Regression Classifier
- Learns word–sentiment associations
- Outputs probability-based predictions
- Uses **class weighting** to handle imbalanced sentiment distribution
- Efficient, interpretable, and well-suited for large text datasets

---

## ⚙️ Machine Learning Pipeline

A unified `sklearn` pipeline ensures:
- No data leakage
- Consistent preprocessing during training and testing
- Cleaner and reproducible experimentation

Pipeline Components:
1. Text Cleaning
2. TF-IDF Vectorization
3. Logistic Regression Classification

---

## 📈 Model Evaluation

The model is evaluated using:
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix**

These metrics provide a balanced view of performance beyond raw accuracy, especially for imbalanced datasets.

---

## 🔍 Key Insights

- Bigram features significantly improve sentiment detection
- Logistic Regression performs well for large-scale text classification
- Proper preprocessing and pipelines are critical for correctness
- Accuracy alone is misleading without precision and recall analysis

---

## ⚠️ Limitations

- Does not capture deep context or sarcasm
- Negation handling is limited
- Performance depends on vocabulary quality
- Classical NLP approach (not transformer-based)

---

## 🚀 Future Improvements

- Upgrade to **BERT / Transformer-based models**
- Add sarcasm and negation awareness
- Perform aspect-based sentiment analysis
- Deploy as a real-time sentiment analysis API
- Integrate visual dashboards for business insights

---

## 🧪 Technologies Used

- Python
- Pandas
- Scikit-learn
- NLP (TF-IDF)
- Logistic Regression
- Google Colab

---

## 👤 Author

**Shiva Abhigna Kanukanti**  
Graduate Student, Computer Science  
Virginia Commonwealth University

---

## 🏁 Conclusion

This project demonstrates how classical NLP techniques combined with a well-structured machine learning pipeline can deliver reliable sentiment classification at scale.  
It provides a strong foundation for advancing toward deep learning–based NLP systems and real-world deployment.

