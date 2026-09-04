# Fake Job Posting Detection Using NLP and Machine Learning

## Project Overview

This project focuses on detecting fraudulent job postings using Natural Language Processing (NLP) and Machine Learning techniques.

The system analyzes the textual information in job postings and classifies them into two categories:

* 0 – Real Job Posting
* 1 – Fraudulent Job Posting

## Problem Statement

Fake job postings can mislead job seekers and may result in financial loss or other risks. This project aims to develop a machine learning model that can identify whether a job posting is real or fraudulent based on its textual content.

## Objectives

* Analyze a dataset containing real and fraudulent job postings.
* Clean and preprocess job-posting text using NLP techniques.
* Extract useful features from text using TF-IDF.
* Train machine learning models for classification.
* Evaluate the models using standard classification metrics.
* Compare the performance of different models.

## Dataset

The project uses the Fake Job Postings Dataset.

The dataset contains information such as:

* Job title
* Location
* Department
* Salary range
* Company profile
* Job description
* Requirements
* Benefits
* Employment type
* Required experience
* Required education
* Industry
* Function
* Fraudulent label

The target variable is `fraudulent`.

* `0` = Real
* `1` = Fraudulent

## Methodology

The project follows this workflow:

```text
Dataset
   ↓
Data Preparation
   ↓
Missing Value Handling
   ↓
Text Combination
   ↓
NLP Preprocessing
   ↓
TF-IDF Feature Extraction
   ↓
Train/Test Split
   ↓
Machine Learning
   ↓
Prediction
   ↓
Evaluation
```

## NLP Techniques Used

The following preprocessing techniques are used:

1. Lowercasing
2. URL removal
3. Email removal
4. Number removal
5. Punctuation removal
6. Tokenization
7. Stopword removal
8. Lemmatization

The following text fields are combined for NLP processing:

* `title`
* `company_profile`
* `description`
* `requirements`
* `benefits`

## Feature Extraction

TF-IDF (Term Frequency–Inverse Document Frequency) is used to convert the processed job-posting text into numerical features.

Unigram and bigram features are used for feature extraction.

## Machine Learning Models

### Logistic Regression

Logistic Regression is used as the primary classification model to predict whether a job posting is real or fraudulent.

### Naive Bayes

Multinomial Naive Bayes is used as a second model to compare its performance with Logistic Regression.

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Classification Report
* Confusion Matrix

## Results

The performance of Logistic Regression and Naive Bayes is compared using the evaluation metrics above.

The actual model results and graphs are available in the project notebook.

## Limitations

* The dataset contains more real job postings than fraudulent job postings.
* The model mainly focuses on textual information.
* Some fraudulent job postings may use language similar to legitimate postings.
* Text-based classification may not identify every type of fraudulent job posting.

## Future Scope

The project can be improved by:

* Exploring LSTM and GRU models.
* Exploring CNN models for text classification.
* Using Transformer-based models.
* Using BERT and other pre-trained language models.
* Combining textual features with other job-posting information.
* Developing a real-time fraud detection application.

## Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn
* Joblib
* Google Colab

## Project Files

```text
Fake-Job-Posting-Detection/
│
├── fake_job_postings.csv
├── fake_job_detection.ipynb
├── requirements.txt
├── README.md
│
├── screenshots/
│
└── report/
```

## Conclusion

This project demonstrates how Natural Language Processing and Machine Learning can be used to detect fraudulent job postings. Text preprocessing and TF-IDF feature extraction are applied to job-posting data, followed by machine learning classification and evaluation.
