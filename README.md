# ❤️ Heart Disease UCI Classification
### Machine Learning Project – Classification Problem


---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Objectives](#objectives)
4. [Data Preprocessing](#data-preprocessing)
5. [Models Compared](#models-compared)
6. [Evaluation Metrics](#evaluation-metrics)
7. [Results](#results)
8. [Presentation](#presentation)
9. [How to Run](#how-to-run)
10. [Acknowledgements](#acknowledgements)
11. [License](#license)
12. [توضیحات فارسی](#توضیحات-فارسی)

---

## Project Overview

This project applies multiple **classification algorithms** to predict the presence and severity of **heart disease** using the **UCI Heart Disease dataset**.  

The pipeline includes:
- Exploratory Data Analysis (EDA)
- Preprocessing and handling missing data
- Feature scaling & encoding
- Training and comparing several models
- Hyperparameter tuning with cross-validation
- Evaluating models with multiple metrics

---

## Dataset

[- **Source:** [UCI Machine Learning Repository – Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease) and [Kaggle](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)  
- **Instances:** 920 rows  
- **Features:** 15 attributes + target (`num`)  
- **Feature types:**  
  - `int64` – 3 columns  
  - `float64` – 5 columns  
  - `object` – 8 columns (categorical)
- **Target variable:** `num` (0 = no disease, 1–4 = disease severity)

---

## Objectives

From your presentation, the main goals were:
- Compare performance of an **MLP neural network** and traditional classifiers (Logistic Regression, Decision Tree, Random Forest, SVM, etc.)
- Investigate **model sensitivity** to MLP hidden layer neuron count
- Train, tune, and evaluate models using cross-validation
- Analyze feature importance and the effect of preprocessing

---

## Data Preprocessing

Performed steps:
- Checked for nulls & inspected data types
- **Imputation** (median or most frequent for missing values)
- **Encoding categorical variables** (One-Hot Encoding)
- **Scaling** numeric features (StandardScaler / MinMaxScaler)
- **Outlier handling** (clipping/extreme removal where needed)
- Splitting into training/testing sets

---

## Models Compared

- **Logistic Regression**
- **SVM (linear, RBF)**
- **Decision Tree**
- **Random Forest**
- **MLPClassifier (Neural Network)**
- **Naive Bayes**
- **Bagging**
- **Voting Classifier**
  
MLP hidden layer sizes tested for sensitivity analysis.

---

## Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC–AUC score  
- Confusion Matrix

Cross-validation (k-fold) used for robust performance comparison.

---

## Results

- Best performing models (highest overall metrics) were **MLP with tuned hidden layers**, **Random Forest**, and **SVM**
- ROC–AUC was >0.9 for several models, indicating strong separability
- Scaling numeric features and proper encoding improved most model scores
- The presentation contains full tables & plots of comparisons

---

## Presentation

Full detailed Persian presentation is included: [`presentation.pdf`](presentation.pdf)

---

## How to Run

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Arianafshar2003/Heart-Disease-UCI-Classification.git
    cd Heart-Disease-UCI-Classification
    ```
2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3. **Open the notebook:**
    ```bash
    jupyter notebook code.ipynb
    ```
4. Run all cells to recreate analysis and results.

---


## توضیحات فارسی

در این پروژه، دیتاست Heart Disease UCI برای پیش‌بینی وجود یا شدت بیماری قلبی استفاده شده است. مراحل شامل:
1. تحلیل اکتشافی داده‌ها (EDA)  
2. پیش‌پردازش شامل جایگزینی مقادیر گمشده، نرمال‌سازی و کدگذاری متغیرهای دسته‌ای  
3. مقایسه مدل‌های مختلف شامل شبکه عصبی MLP و الگوریتم‌های طبقه‌بندی سنتی  
4. ارزیابی با دقت، دقت مثبت، بازیابی، F1 و ROC–AUC  
نتایج کامل در فایل [presentation.pdf](presentation.pdf) موجود است.

---
