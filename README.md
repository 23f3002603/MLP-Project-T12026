# Comment Category Prediction using Machine Learning

## Project Overview

This project was developed as part of the **Machine Learning Practice (MLP)** coursework in the BS Degree Program at Indian Institute of Technology Madras.

The project focuses on predicting how an online platform categorizes user-generated comments using textual content, engagement metrics, symbolic indicators, and metadata features.

The work involved:

* exploratory data analysis,
* NLP preprocessing,
* feature engineering,
* model experimentation,
* and hyperparameter tuning over nearly two months.

---

# Competition Overview

The project was based on the **Comment Category Prediction Challenge** hosted on [Kaggle](https://www.kaggle.com?utm_source=chatgpt.com).

The challenge required participants to analyze short textual comments and predict the final moderation or categorization label assigned by the platform.

The dataset combines:

* text data,
* user interaction signals,
* hidden internal indicators,
* symbolic expression features,
* and topic reference metadata.

---

# Problem Statement

Given a dataset containing:

* comment text,
* engagement statistics,
* emoticon indicators,
* demographic/topic reference signals,
* and internal platform-generated features,

the objective was to build a machine learning pipeline capable of accurately classifying comments into one of four target categories.

---

# Dataset Description

The dataset consists of:

* `train.csv`

  * Contains feature columns along with the target label.

* `test.csv`

  * Contains feature columns without labels for prediction.

* `sample_submission.csv`

  * Sample submission file for Kaggle evaluation.

---

# Features Used

## Textual Feature

* `comment`

  * Raw textual content of the comment.

## Temporal Feature

* `created_date`

  * Timestamp indicating when the comment was posted.

## Interaction Features

* `upvote`
* `downvote`

## Emoticon Features

* `emoticon_1`
* `emoticon_2`
* `emoticon_3`

## Metadata / Indicator Features

* `race`
* `religion`
* `gender`
* `disability`

## Internal Platform Features

* `if_1`
* `if_2`

## Target Variable

* `label`

  * Final category assigned by the platform.

---

# Project Workflow

## 1. Exploratory Data Analysis (EDA)

Performed:

* class distribution analysis,
* missing value inspection,
* text length analysis,
* interaction feature analysis,
* and feature correlation exploration.

---

## 2. NLP Preprocessing

Applied:

* lowercasing,
* punctuation removal,
* stopword filtering,
* TF-IDF vectorization,
* and n-gram extraction.

---

## 3. Feature Engineering

Created additional features such as:

* comment length,
* word count,
* vote ratios,
* vote difference,
* total reactions,
* and combined symbolic indicators.

---

# Machine Learning Models

The following models were explored and compared:

* Logistic Regression
* Linear SVM (`LinearSVC`)
* SGD Classifier
* Multinomial Naive Bayes
* LightGBM (`LGBMClassifier`)

---

# Hyperparameter Tuning

Hyperparameter optimization was performed using:

* `GridSearchCV`
* Cross-validation
* Macro F1-score evaluation

---

# Final Results

## Kaggle Leaderboard Score

* **0.76262**

## Validation Macro F1 Score

* **0.7637**

## Course Grade

* **A Grade**

---

# Technologies Used

## Language

* Python

## Libraries

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* LightGBM

---

# Repository Structure

```text id="ghz6n6"
project/
│
├── notebook.ipynb
├── README.md
├── requirements.txt
├── images/
└── dataset_links.txt
```

---

# Key Learnings

This project provided hands-on experience in:

* end-to-end ML workflow development,
* NLP preprocessing,
* feature engineering,
* model evaluation,
* hyperparameter tuning,
* and Kaggle competition pipelines.

---

# Future Improvements

Potential improvements include:

* transformer-based NLP models,
* BERT embeddings,
* ensemble learning,
* advanced feature extraction,
* and deeper error analysis.

---

# License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

# Author

Tathagata Banerjee
BS Data Science Student
Indian Institute of Technology Madras
