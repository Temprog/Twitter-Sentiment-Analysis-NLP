# Twitter Sentiment Analysis and Prediction  

This project focuses on analyzing Twitter tweets and classifying them into three sentiment categories: **Positive, Negative, and Neutral**.  
It also includes a prediction component that applies the best-performing machine learning model to classify the sentiment of new feedback and review tweets.  

---

## 📊 Dataset  

The dataset `twitter_sample.csv` contains:  

- `feedback`: The text of the tweet  
- `label`: The sentiment label (Positive, Negative, Neutral)  

---

## 🤖 Models & Performance  

| Model                        | Accuracy (%) |
|-------------------------------|--------------|
| Logistic Regression           | **67.85**    |
| Random Forest Classifier      | **78.75**    |
| Support Vector Machine (SVM)  | **70.83**    |
| Multinomial Naive Bayes       | **61.83**    |
| Bernoulli Naive Bayes         | **63.81**    |
| Gradient Boosting             | **50.91**    |

➡️ **Random Forest Classifier achieved the best performance.**

---

## 📈 Visualizations  

- [Confusion Matrix](https://github.com/Temprog/Twitter-Sentiment-Analysis-NLP/blob/main/visualizations/confusion_matrix_svm.png)
- [Sentiment Distribution (Bar Chart, Pie Chart](https://github.com/Temprog/Twitter-Sentiment-Analysis-NLP/blob/main/visualizations/sentiment_distribution.png)
- [Word Cloud of frequent terms](https://github.com/Temprog/Twitter-Sentiment-Analysis-NLP/blob/main/visualizations/wordcloud.png)
- [Model Accuracy Comparison (bar chart)](https://github.com/Temprog/Twitter-Sentiment-Analysis-NLP/blob/main/visualizations/model_accuracy.png)
- [Predicted Sentiment Distribution (New Reviews Data)](https://github.com/Temprog/Twitter-Sentiment-Analysis-NLP/blob/main/visualizations/predicted_sentiment.png)

---

## 📌 Project Workflow  

The workflow includes:  

- **Data Loading & Preprocessing**  
  - Clean text (remove URLs, mentions, hashtags, special characters, lowercase conversion)  
  - Tokenization, stopword removal, and lemmatization  
  - Handle missing values and irrelevant columns  

- **Exploratory Data Analysis (EDA)**  
  - Visualize sentiment distribution  
  - Word frequency analysis via word clouds  

- **Feature Extraction**  
  - TF-IDF Vectorization  

- **Modeling & Evaluation**  
  - Models trained: Logistic Regression, Random Forest, SVM, Multinomial Naive Bayes, Bernoulli Naive Bayes, Gradient Boosting  
  - Evaluation with accuracy, classification reports and confusion matrices  

- **Prediction on New Data**  
  - The best-performing model (Random Forest Classifier) is used to predict sentiments on new review tweets.  

---

## ⚙️ Steps to Reproduce  

1. **Google Colab** (recommended):  
   - Upload `twitter_sample.csv` and `cat.png` to Google Drive  
   - Update file paths in the notebook  
   - Run cells sequentially  

2. **Local Setup**:  
   ```bash
   git clone https://github.com/yourusername/twitter-sentiment-analysis.git
   cd twitter-sentiment-analysis
   pip install -r requirements.txt

---

## 🌟 Importance of the Project

This project demonstrates how Natural Language Processing (NLP) and machine learning can be applied to:

- Analyze public opinion on social platforms
- Automate sentiment classification for large-scale feedback
- Provide actionable insights for businesses, policymakers and researchers

---

## ⚠️ Limitations

- Dataset size: Small sample, may not generalize well
- Imbalanced classes: Some sentiments may dominate the dataset
- Limited feature representation: TF-IDF only; could be improved with word embeddings (Word2Vec, BERT, etc.)
- Context understanding: Traditional ML models may misinterpret sarcasm, irony, or nuanced sentiments
