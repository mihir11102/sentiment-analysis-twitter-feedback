# Sentiment Analysis on Twitter Feedback

A machine learning project that analyses public sentiment from Twitter data using **Natural Language Processing (NLP)** techniques. The model classifies tweets as positive, negative, or neutral to uncover patterns and trends in online discussions.

---

## 🧠 Project Overview
Social media provides valuable insights into public opinion. This project applies text preprocessing, tokenisation, feature extraction, and sentiment classification to Twitter feedback. Models such as Logistic Regression, Naïve Bayes, and Support Vector Machines are compared for performance. The objective is to automate sentiment detection and provide an interpretable NLP pipeline for text analytics applications.

🔧 System Architecture




<img width="731" height="201" alt="Untitled Diagram drawio (2)" src="https://github.com/user-attachments/assets/8331dbbf-d364-4375-9475-c1704e73053c" />

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

Model Evaluation

This project evaluates two sentiment classification approaches: a classical machine learning baseline using TF-IDF features, and a fine-tuned DistilBERT transformer model. Both were trained and tested on cleaned Twitter data, with performance assessed using accuracy, precision, recall, and F1-scores.

1. Logistic Regression (TF-IDF Baseline)

The baseline model uses TF-IDF vectorisation with Logistic Regression. It is lightweight, interpretable, and provides a strong starting point for comparison.

Key observations

Strong performance on negative sentiment

Lower recall for positive tweets due to class imbalance

Coefficient weights highlight influential terms such as sucks, love, great, and tired


<img width="548" height="455" alt="confusion_matrix" src="https://github.com/user-attachments/assets/1a3211ce-b97e-4150-ae97-4d1790c0a782" />



2. DistilBERT Transformer Model

DistilBERT captures contextual meaning more effectively than TF-IDF, making it better suited for informal, noisy, and ambiguous Twitter text.

Key observations

Higher overall accuracy (approximately 0.88)

Considerably improved recall for positive tweets

More stable performance on short or subtle emotional signals

Better handling of slang, misspellings, and multi-word dependencies





<img width="699" height="470" alt="training_loss" src="https://github.com/user-attachments/assets/12d3eb28-7227-4309-8657-6e5c4a441cf8" />


3. Performance Summary
| Model                         | Accuracy | Precision (Neg/Pos) | Recall (Neg/Pos) | F1 (Neg/Pos) | Notes |
|------------------------------|----------|----------------------|-------------------|---------------|-------|
| Logistic Regression (TF-IDF) | 0.83     | 0.85 / 0.71          | 0.94 / 0.45       | 0.89 / 0.55   | Strong baseline but affected by class imbalance |
| DistilBERT Transformer       | 0.88     | 0.88 / 0.72          | 0.93 / 0.59       | 0.90 / 0.65   | Better contextual understanding and generalisation |




4. Explainability and Interpretation

Several interpretability tools were used to understand how the models made their predictions.

SHAP values highlight the contribution of individual tokens

Coefficient-based plots show the strongest positive and negative indicators for the TF-IDF model

Word-influence maps make sentiment decisions easier to interpret visually

<img width="790" height="940" alt="shap_summary" src="https://github.com/user-attachments/assets/12c21ecf-5b90-4c48-ab29-1f8e06ccd7cb" />


5. Insights

DistilBERT provides stronger balance across classes and reduces false negatives

The baseline model remains useful because of its clarity and speed

Mixed-tone, sarcastic, or context-dependent tweets remain challenging for both models

Imbalanced data still affects positive-class performance and could be improved through augmentation or resampling
.

## 🔁 Reproducibility

All dependencies are listed in requirements.txt. The notebook runs with Python 3.10+ and common ML/NLP libraries such as pandas, nltk, scikit-learn, and matplotlib. A fixed random seed ensures reproducibility of results.

## 👨‍💻 Author

Mihir Bhansali
