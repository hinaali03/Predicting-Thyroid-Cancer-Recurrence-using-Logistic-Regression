# 🧠 Predicting Thyroid Cancer Recurrence using Logistic Regression

A machine learning project that predicts the recurrence of thyroid cancer in patients using a logistic regression model. The dataset was sourced from **Kaggle**.

---

## 📁 Project Overview

This project demonstrates the complete machine learning workflow:
- Cleaning and preprocessing real-world clinical data
- Encoding categorical variables
- Training a logistic regression model
- Evaluating the model using classification metrics and visualizations

---

## 📊 Dataset

- **Source**: [Kaggle - Differentiated Thyroid Cancer Recurrence Dataset]([https://www.kaggle.com/](https://www.kaggle.com/datasets/alsaniipe/differentiated-thyroid-cancer-recurrence-dataset)) 
- **File used**: `Thyroid_Diff.csv`
- Features include:
  - Gender, Smoking history, Radiotherapy, Pathology type
  - TNM Staging (T, N, M)
  - Focality, Adenopathy, Stage, Risk category
  - Recurrence outcome (`Recurred`: Yes/No)

---

## 🧼 Data Preprocessing

- Handled missing values and categorical encoding using `map()`
- Removed non-predictive or irrelevant columns:
  - `'Thyroid Function'`
  - `'Physical Examination'`
- Transformed variables like `Gender`, `Smoking`, `T`, `N`, `M`, `Pathology`, etc. into numerical formats

---

## 🤖 Model Building

- Split data into **train** and **test** sets (80/20)
- Used `Pipeline` to combine:
  - `StandardScaler()` for feature normalization
  - `LogisticRegression()` for classification
- Hyperparameter tuning using `RandomizedSearchCV` with:
  - C (regularization strength)
  - L2 penalty

---

## 📈 Model Evaluation

- Best parameters and cross-validation score printed
- Evaluated performance using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)
- Visualized confusion matrix with `seaborn`

---

## 🔍 Results

- ✅ **Accuracy**: _(shown in output)_
- 📉 Confusion Matrix: Clearly shows predicted vs. actual recurrence
- 📄 Classification Report: Provides class-wise performance metrics

---

## 🛠️ Technologies Used

- 🐍 Python (Pandas, NumPy, Matplotlib, Seaborn, scikit-learn)
- 📊 Logistic Regression for classification
- 📁 Jupyter Notebook (for interactive development)

---



---

## ⚠️ Disclaimer

This project is for **academic and educational purposes** only. The predictions are based on a public dataset and do not substitute for professional medical advice or diagnosis.

