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
🚀 How to Run

Clone this repository:

git clone https://github.com/mihir11102/sentiment-analysis-twitter-feedback.git
cd sentiment-analysis-twitter-feedback


Install the dependencies:

pip install -r requirements.txt


Launch Jupyter Notebook:

jupyter notebook setup.ipynb


Run the cells step-by-step to:

Load and clean the dataset

Tokenise and vectorise text

Train and evaluate machine learning models

Visualise sentiment distribution and accuracy

📊 Results

The trained model achieves high accuracy in distinguishing between positive and negative sentiments. Visual outputs include:

Confusion matrix and classification metrics

Word frequency and sentiment distribution plots

(You can replace this section with actual performance metrics once your model is finalised.)

🧠 Future Improvements

Fine-tune transformer models such as BERT for better accuracy

Extend dataset to multilingual sentiment analysis

Deploy as a simple web dashboard or REST API

👨‍💻 Author

Mihir Bhansali
Graduate Student | Data Science & AI | University of Florida
📫 GitHub

🪶 License

This project is open-source and available under the MIT License.

⚡ Note: The dataset is stored using Git LFS. To access or share the repository, ensure Git LFS is installed and configured on your system.
