🛡️ Cyberbullying Detection using Machine Learning & NLP
📌 Project Overview

This project focuses on detecting and classifying cyberbullying content from social media text using Natural Language Processing (NLP) and Machine Learning techniques.

The system preprocesses tweets, converts them into numerical features using TF-IDF, and trains multiple classification models to identify different types of cyberbullying.

🎯 Objectives

Detect cyberbullying in social media text

Classify tweets into different bullying categories

Compare performance of multiple ML models

Improve accuracy using ensemble learning (Stacking)

📊 Dataset Used

Source: Kaggle

Dataset: Cyberbullying Classification Dataset

Classes:

age

gender

religion

ethnicity

other_cyberbullying

not_cyberbullying

🧹 Data Preprocessing Steps

The project applies a full NLP pipeline:

Removed duplicates and checked null values

Lowercasing text

Removed punctuation

Removed stopwords (NLTK)

Tokenization

Lemmatization

Stemming

Removed numbers

Removed accents

Rejoined tokens into final processed text

🔤 Feature Engineering

Used TF-IDF Vectorization

max_features = 5000

ngram_range = (1,2) (unigrams + bigrams)

min_df = 3

max_df = 0.9

🤖 Machine Learning Models Used

The following models were trained and compared:

Naive Bayes

Support Vector Machine (Linear SVM)

Random Forest

📈 Model Accuracy

Naive Bayes → 78.03%

SVM → 82.46%

Random Forest → 82.38%

🧠 Ensemble Learning (Advanced)

A Stacking Classifier was implemented to improve performance:

Base Learners:

Naive Bayes

Linear SVM

Random Forest

Meta Learner:

Logistic Regression

🚀 Final Accuracy (Stacking Model)

84.46%

This was the best performing model.

📊 Visualizations

Confusion Matrix for each model

WordClouds for each cyberbullying category

These help in understanding:

Prediction performance

Common words in each bullying type

🛠️ Technologies & Libraries

Python

Google Colab

pandas

numpy

nltk

scikit-learn

matplotlib

seaborn

wordcloud

kagglehub

⚙️ Project Workflow

Download dataset from Kaggle

Clean and preprocess text

Apply NLP transformations

Convert text → TF-IDF features

Train ML models

Evaluate performance

Improve using stacking ensemble

📂 Project Structure
cyberbullying-detection/
│
├── cyberbullying_detection.ipynb
├── README.md

💡 Key Learnings

Practical use of NLP in real-world problems

Text preprocessing pipeline

TF-IDF feature extraction

Model comparison techniques

Ensemble learning using stacking

🔮 Future Improvements

Use deep learning models (LSTM/BERT)

Deploy as a web app

Real-time cyberbullying detection

Improve detection of "not_cyberbullying" class

👩‍💻 Author

Mahi Sinha

CSE Student

Interested in AI, ML & NLP

Smart India Hackathon Participant
