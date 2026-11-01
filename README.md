# SMS Spam Detection with Naive Bayes and TF-IDF

![scikit-learn](https://img.shields.io/badge/scikit--learn-Naive%20Bayes-f7931e)
![NLTK](https://img.shields.io/badge/NLTK-preprocessing-informational)

This project classifies SMS messages as spam or legitimate ("ham") with a classic text pipeline: NLTK preprocessing, TF-IDF features and Naive Bayes. It compares the Gaussian, Multinomial and Bernoulli variants. For a spam filter, **precision** matters most, because a false positive hides a real message.

## Pipeline

1. **Data:** the [SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection) (`Data/spam.csv`): unused columns are dropped and duplicates removed.
2. **EDA:** class balance, and message length in characters, words and sentences by class, plus word clouds.
3. **Preprocessing:** lower-casing, tokenization, removal of special characters, stop-words and punctuation, then stemming.
4. **Features:** TF-IDF, with the vocabulary size (`max_features`) tuned.
5. **Models:** Gaussian, Multinomial and Bernoulli Naive Bayes.

## Result

Multinomial Naive Bayes on TF-IDF features gives **97% accuracy with 100% precision** on the held-out set: no legitimate message is flagged as spam.

## Run

```bash
pip install pandas numpy scikit-learn nltk matplotlib seaborn wordcloud
jupyter notebook "Spam Detection.ipynb"
```
