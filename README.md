# Vegan Food Sentiment Analysis | NLP Project

## Overview
This project analyzes public sentiment toward vegan food using Twitter data. Tweets are collected using the Twitter API and processed using Natural Language Processing (NLP) techniques. Machine Learning models are then applied to classify sentiments into Positive, Negative, and Neutral categories.

The goal is to understand public perception of vegan food across different countries (India, USA, Canada).

---

## Problem Statement
Social media platforms contain large amounts of unstructured text data. Understanding public sentiment about vegan food can help:

- Food industry stakeholders understand consumer perception  
- Researchers analyze dietary trends  
- Businesses improve marketing strategies  

This project builds a sentiment analysis system to classify tweets related to vegan food into sentiment categories.

---

## Dataset
- Source: Twitter API (Tweepy)
- Keywords: vegan, food, diet
- Countries:
  - India
  - United States
  - Canada
- Data fields:
  - Tweet text
  - Location
  - Likes and retweets
  - Timestamp

---

## Project Workflow

### 1. Data Collection
- Extracted tweets using Tweepy API
- Filtered by keywords and geolocation
- Stored in structured format (CSV)

### 2. Data Preprocessing
- Removed mentions, hashtags, URLs, punctuation
- Converted text to lowercase
- Removed stopwords
- Applied POS tagging
- Lemmatization

### 3. Feature Engineering
- TF-IDF Vectorization
- Count Vectorization

### 4. Sentiment Labeling
- Used VADER Sentiment Analyzer
- Classified tweets as:
  - Positive
  - Neutral
  - Negative

### 5. Model Building
Models used:
- Support Vector Machine (SVC)
- K-Nearest Neighbors (KNN)
- Random Forest
- Naive Bayes

### 6. Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Precision, Recall, F1-score

---

## Model Performance

### TF-IDF Vectorizer Results

| Model          | Accuracy |
|----------------|----------|
| SVC            | 55.81%   |
| KNN            | 51.16%   |
| Random Forest  | 69.76%   |
| Naive Bayes    | 72.09%   |

### Count Vectorizer Results

| Model          | Accuracy |
|----------------|----------|
| SVC            | 69.76%   |
| KNN            | 41.86%   |
| Random Forest  | 60.46%   |
| Naive Bayes    | 53.48%   |

---

## Key Insights
- Most tweets are neutral in sentiment
- Positive sentiment is higher in US and Canada compared to India
- Discussions often revolve around health, diet, and plant-based lifestyle
- Negative sentiment is mostly linked to processed vegan food debates

---

## Technologies Used
- Python
- Tweepy (Twitter API)
- NLTK (Natural Language Processing)
- Scikit-learn (Machine Learning)
- Pandas, NumPy (Data Processing)
- Matplotlib, Seaborn (Visualization)
- WordCloud

---

## Machine Learning Pipeline
- Text Cleaning
- Tokenization
- Lemmatization
- Feature Extraction (TF-IDF / CountVectorizer)
- Model Training
- Evaluation

---

## How to Run This Project

### 1. Install Dependencies

pip install pandas numpy nltk tweepy scikit-learn matplotlib seaborn wordcloud

### 2. Run Notebook
Open Jupyter Notebook and execute:

Vegan_Food_Sentiment_Analysis.ipynb

### 3. Twitter API Setup
Create a `keys.ipynb` file with:

API_key = "your_key"
API_key_secret = "your_secret"
Access_token = "your_token"
Access_token_secret = "your_token_secret"


---

## Future Improvements
- Use deep learning models (LSTM, BERT)
- Deploy using Streamlit or Flask
- Improve class imbalance handling
- Add real-time Twitter streaming analysis
- Build interactive dashboard

---

## Author
Neha Patel  
Data Analyst | Python | SQL | Power BI | Machine Learning
