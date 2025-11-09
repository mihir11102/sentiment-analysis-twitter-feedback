# Sentiment Analysis on Twitter Feedback

A machine learning project that analyses public sentiment from Twitter data using **Natural Language Processing (NLP)** techniques. The model classifies tweets as positive, negative, or neutral to uncover patterns and trends in online discussions.

---

## 🧠 Project Overview
Social media provides valuable insights into public opinion. This project applies text preprocessing, tokenisation, feature extraction, and sentiment classification to Twitter feedback. Models such as Logistic Regression, Naïve Bayes, and Support Vector Machines are compared for performance. The objective is to automate sentiment detection and provide an interpretable NLP pipeline for text analytics applications.

---

## ⚙️ Installation and Setup
1. Clone this repository:
   ```bash
     git clone https://github.com/mihir11102/sentiment-analysis-twitter-feedback.git
     cd sentiment-analysis-twitter-feedback
2. Install the required dependencies:

pip install -r requirements.txt


3. Ensure Git LFS is installed to fetch large dataset files:

git lfs install
git lfs pull

## ▶️ How to Run the Notebook

Launch Jupyter Notebook:

jupyter notebook setup.ipynb

Download Model (Important)

The model files are not stored in the GitHub repository because they exceed the size limits.
Please download the model folder from Google Drive:

Download link:
https://drive.google.com/drive/folders/1l7mbzOSQV1uPQPJ7p9lAU0dgzvo248Ag

After downloading, unzip the folder and place it in the following directory inside the project:

sentiment-analysis-twitter-feedback/
│
├── models/
│   └── distilbert_sentiment_model/
│       ├── config.json
│       ├── model.safetensors
│       ├── tokenizer.json
│       ├── tokenizer_config.json
│       ├── vocab.txt
│       └── special_tokens_map.json



Open setup.ipynb and execute all cells sequentially:

Load and clean the dataset

Perform text preprocessing and vectorisation

Train and evaluate sentiment classification models

Visualise accuracy, confusion matrix, and key metrics


## 📊 Dataset Information

File: data/Machine Learning Sentiment.csv

Size: ~228 MB (tracked using Git LFS)

Content: Tweets labelled as positive, negative, or neutral

Source: Publicly available Twitter dataset for academic sentiment analysis

Note: Git LFS must be configured to correctly retrieve large files. Learn more at Git LFS
.

## 🔁 Reproducibility

All dependencies are listed in requirements.txt. The notebook runs with Python 3.10+ and common ML/NLP libraries such as pandas, nltk, scikit-learn, and matplotlib. A fixed random seed ensures reproducibility of results.

## 👨‍💻 Author

Mihir Bhansali
