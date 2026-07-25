# 🏥 Health Risk Prediction Using Machine Learning

## 📖 Project Overview

This project focuses on predicting an individual's health condition based on lifestyle and wellness indicators such as:

- Sleep Duration
- Heart Rate
- BMI
- Diet Type
- Stress Level
- Physical Activity
- Exercise Duration
- Water Intake
- Smoking & Alcohol Habits

The goal is to classify people into:

✅ Fit

⚠️ At-Risk

🚨 Unhealthy

using Machine Learning and Feature Engineering techniques.

---

## 🎯 Business Problem

Healthcare organizations and wellness platforms collect large amounts of lifestyle data.

Identifying individuals at risk of future health problems enables early intervention and personalized wellness recommendations.

This project develops a predictive analytics solution capable of automatically categorizing individuals based on health risk.

---

## 📊 Dataset Information

| Metric | Value |
|----------|---------|
| Records | 93,300 |
| Features | 20 |
| Target Classes | 3 |
| Domain | Healthcare Analytics |

### Target Variable

- Fit
- At-Risk
- Unhealthy

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- CatBoost
- Google Colab

---

## 🔍 Exploratory Data Analysis

Performed:

- Missing Value Analysis
- Duplicate Detection
- Statistical Summary
- Distribution Analysis
- Outlier Detection
- Class Distribution Analysis
- Bivariate Analysis

Key findings:

- Stress Level strongly influences health status.
- Sleep Duration is one of the most important predictors.
- Physical Activity impacts overall health outcomes.
- BMI has significant predictive importance.

---

## ⚙️ Feature Engineering

Created custom healthcare indicators:

### BMI Category

- Underweight
- Normal
- Overweight
- Obese

### Activity Score

```python
step_count * exercise_duration
```

### Sleep Score

```python
sleep_duration * sleep_quality_score
```

### Health Risk Score

```python
heart_rate + bmi - sleep_duration
```

### Calories Per Step

```python
calorie_expenditure / step_count
```

### Water Per Exercise

```python
water_intake / exercise_duration
```

---

## 🤖 Machine Learning Model

Model Used:

✅ CatBoost Classifier

Parameters:

```python
iterations=300
learning_rate=0.1
depth=6
loss_function='MultiClass'
```

---

## 📈 Results

| Metric | Value |
|----------|----------|
| Algorithm | CatBoost |
| Classes | 3 |
| Best Iteration | 266 |
| Validation F1 Score | 96.74% |

---

## 🔥 Most Important Features

Feature importance analysis identified:

1. Stress Level
2. Sleep Duration
3. Physical Activity Level
4. BMI
5. Heart Rate
6. Smoking & Alcohol Habits

These variables contributed most to health-condition prediction.

---

## 📂 Project Workflow

Data Collection
↓
Data Cleaning
↓
Missing Value Treatment
↓
EDA
↓
Feature Engineering
↓
Data Validation
↓
Train Validation Split
↓
CatBoost Model Training
↓
Feature Importance Analysis
↓
Prediction Generation

---

## 📌 Future Improvements

- Hyperparameter tuning
- XGBoost comparison
- LightGBM implementation
- SHAP Explainability
- Streamlit Web App
- Real-Time Prediction Dashboard

---

https://github.com/akkikoomar27/health-risk-prediction-catboost/blob/main/Predicting_Student_Health_Risk.ipynb

## 👨‍💻 Author

Akhilesh Yadav

Data Analyst | Data Scientist

Skills:
Python | SQL | Power BI | Machine Learning | Snowflake | SSIS | Azure SQL
