# Email Spam Classifier (TF-IDF + ML)

This project builds an **Email Spam Detection** model using classical machine learning with **TF-IDF text features**.  
It compares multiple models (e.g., **Naive Bayes** and **Logistic Regression**) to classify messages as **Spam** or **Not Spam**.

---

## Project Goal

Given an email/text message, predict whether it is:
- **Spam (1)** or
- **Not Spam (0)**

---

## Dataset

- File: `spam_or_not_spam.csv`
- Target column: typically `label` (0/1)
- Text column: typically `email` (message content)

> If your column names are slightly different, update them in the notebook/script.

---

## What This Project Does

### 1) Data Loading & Cleaning
- Loads the CSV using `pandas`
- Handles missing values (if any)
- Basic checks: shape, duplicates, label distribution

### 2) Text Preprocessing
- Converts text into numeric features using:
  - **TF-IDF Vectorizer** (Term Frequency–Inverse Document Frequency)

### 3) Model Training
Trains and compares models such as:
- **Multinomial Naive Bayes**
- **Logistic Regression**

### 4) Evaluation
Evaluates performance using:
- Accuracy
- Classification report (precision, recall, F1-score)
- Confusion matrix (optional)

---

## How to Run

### Option A — Jupyter Notebook
1. Put the dataset file in the same folder (or update the path in the notebook).
2. Run:
```bash
jupyter notebook
```bash
Create and install dependencies:

pip install -r requirements.txt
```
```bash
requirements.txt:

numpy
pandas
scikit-learn
matplotlib
seaborn
```
