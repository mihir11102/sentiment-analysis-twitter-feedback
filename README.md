# Sentiment Analysis on Twitter Feedback 🧠💬

A machine learning project to analyse public sentiment from Twitter data using **Natural Language Processing (NLP)** techniques. The model identifies whether a tweet expresses a **positive**, **negative**, or **neutral** emotion based on textual patterns and linguistic cues.

---

## 📁 Project Overview
Social media platforms generate vast amounts of text data daily. Analysing this information helps understand public perception toward products, events, or social issues.  
This project leverages NLP methods to perform sentiment analysis on a large dataset of tweets related to a specific topic, enabling insights into audience sentiment trends.

---

## ⚙️ Tech Stack
- **Language:** Python  
- **Frameworks & Libraries:**  
  - pandas, numpy — data manipulation  
  - scikit-learn — feature extraction and model training  
  - nltk / spaCy — text preprocessing and tokenisation  
  - matplotlib, seaborn — visualisation  
- **Tools:** Jupyter Notebook, Git LFS for large file management

---

## 🧾 Dataset
The dataset used for this project (`Machine Learning Sentiment.csv`) contains preprocessed tweets and their sentiment labels.  
Due to its large size, it is tracked using **Git Large File Storage (LFS)**. To access it after cloning:
```bash
git lfs pull
