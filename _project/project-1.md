---
title: "Mental Health Text Classifier"
excerpt: "Deep learning model to detect suicidal ideation in social media text using BERT, CNN-LSTM, and NLP techniques. Built a dataset from Twitter and Reddit for early intervention."
collection: project
image: "/images/Data_challenge.png"
tags:
  - NLP
  - Deep Learning
  - BERT
  - Python
github: "https://github.com/shreeramgs/Data-Challenge-2022-UB"
---

<div style="display: flex; justify-content: center; margin-bottom: 2em;">
  <div 
    style="
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 2px 16px 0 rgba(0,0,0,0.17);
      padding: 2em 2em 1.5em 2em;
      max-width: 720px;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
    "
  >
    <img 
      id="mental-health-img"
      src="/images/Data_challenge.png"
      alt="Mental Health Text Classifier" 
      style="max-width: 480px; width: 90%; height: auto; border-radius: 12px; box-shadow: 0 2px 8px 0 rgba(0,0,0,0.10); margin-bottom: 1em; transition: opacity 0.5s;"
    />
    <h2 style="margin: 0.5em 0 0.2em 0; font-size: 1.5em;">Mental Health Text Classifier</h2>
    <p style="color: #444; margin: 0 0 0.5em 0; font-size: 1em; text-align: center;">
      Deep learning model to detect suicidal ideation in social media text using BERT, CNN-LSTM, and NLP techniques. Built a dataset from Twitter and Reddit for early intervention.
    </p>
  </div>
</div>



### Description
Accurate intervention of suicidal ideation and behavior in depressed people can help them get the therapeutic help and care they need, which can save their lives in many scenarios. The goal is to precisely anticipate data in order to avert incidents such as suicide and to assist people in overcoming depression. 

### Formulation
1. Creation of a dataset from Twitter and Reddit that suicidal thought intention.
2. Preprocess sentences and identify new features from textual data.   
3. Make use of deep learning approaches such as RNN, CNN-LSTM and pre-trained models like BERT to classify text. 

### Dataset
We develop a primary dataset to help us figure out whether someone is suicidal or depressed. This information was taken from Reddit. We collect data from parts of the internet using the Python Reddit API. We scrape from subreddits that relate to depression and suicidal thoughts. We also make use of Twitter API to collect tweets that were tagged suicidal.

### Preprocessing and Feature Extraction
Text data require lot of preprocessing before they could be analyzed or modelled:

* Remove non-English words
* Remove mentions, hashtags, external links 
* Remove stop words
* Stemming, Lemmatization

### Features Used
* Unigrams, Bigrams 
* TF-IDF (term frequency-inverse document frequency)
* LIWC (Linguistic Inquiry and Word Count)
* Sentiment analysis

### Modeling
Suicidal text detection is a supervised binary classification problem. We use machine learning approaches like SVM, XGBoost, and deep learning models (BERT) to classify texts. Accuracy, Precision, Recall and F-1 Score are the evaluation metrics.

### Output
Web application where users can check if text indicates suicidal ideation, with API for third-party integration.
