# Spam detection model using Bayesian modeling and NLP

## Project Overview
This project focuses on developing an SMS spam detection model using Naive Bayes and Natural Language Processing (NLP) techniques. The primary objective is to create a predictive model capable of distinguishing between spam and legitimate SMS messages, thereby improving user experience and communication security.

## Methodology-Implementation
## Data Gathering and Loading
The Kaggle SMS Spam Collection Dataset is employed to acquire a dataset containing English SMS messages labeled as ham (legitimate) or spam.
## Data Cleaning and Exploration
Initial data cleaning involves the removal of unnecessary columns and handling duplicated values.
Exploratory Data Analysis includes visualizing the classification problem and extracting key features like the number of characters, words, and sentences in the messages.
## Data Preprocessing
Text data undergoes preprocessing steps, including lowercase conversion, tokenization, removal of special characters, stopwords, and punctuation.
Additional steps involve stemming and lemmatization for further refinement.
## Building a Model using Naive Bayes
Employing TFIDF vectorization, the project constructs a Multinomial Naive Bayes model.
Comparative analysis is conducted with Gaussian and Bernoulli Naive Bayes models to assess performance.
## Improving the Model
Experimentation involves tweaking parameters, such as max_features in TFIDF, to optimize the model's accuracy and precision.
## Result Achievement
## Model Performance
The final model, a Multinomial Naive Bayes with TFIDF vectorization, achieves remarkable results with a 97% accuracy and 100% precision score.
Continuous experimentation and enhancements contribute to the model's robustness, ensuring an effective SMS spam detection system.
