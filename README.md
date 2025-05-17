# Sentiment Analysis on Movie Reviews

This project focuses on building a sentiment analysis model using a dataset of movie reviews. The goal is to classify each review as either positive or negative based on its text content.

## Project Overview

To efficiently analyze and model the data, I performed the following:

- Sampled 10,000 movie reviews from the full dataset  
- Preprocessed the text data to remove noise  
- Trained and evaluated three Naive Bayes classifiers  
- Compared model performance based on accuracy

## Dataset

The dataset consists of labeled movie reviews. Each entry contains a short review and a sentiment label indicating whether the review is positive or negative.

## Text Preprocessing

The following preprocessing steps were applied to clean and standardize the text:

1. Sampled 10,000 reviews  
2. Removed HTML tags (such as `<br>`, `<i>`)  
3. Removed special characters and digits  
4. Converted all text to lowercase  
5. Removed stopwords (common words that do not carry sentiment)  
6. Applied stemming to reduce words to their base form

## Models Used

Three Naive Bayes models were tested:

- Gaussian Naive Bayes  
- Multinomial Naive Bayes  
- Bernoulli Naive Bayes

## Model Performance

| Model               | Accuracy |
|--------------------|----------|
| GaussianNB          | 0.7945   |
| MultinomialNB       | 0.8460   |
| BernoulliNB         | 0.8470   |

Bernoulli Naive Bayes performed slightly better than the others on this classification task.

## Key Takeaways

- Preprocessing significantly improves sentiment classification accuracy  
- Multinomial and Bernoulli Naive Bayes are better suited for text data than Gaussian  
- Even basic models can produce strong results when paired with a solid NLP pipeline

## Repository Contents

movie-review-sentiment-analysis/  
- sentiment_analysis.ipynb – Main notebook with data processing, model training, and evaluation  
- requirements.txt – List of Python packages used  
- README.md – Project documentation

## About This Project

This project allowed me to apply core Natural Language Processing techniques to a practical machine learning task. It demonstrates my understanding of data preprocessing, feature engineering, and model evaluation in the context of binary text classification.

