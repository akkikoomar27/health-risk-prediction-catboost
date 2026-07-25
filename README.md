# 🏥 Health Risk Prediction Using Machine Learning

Welcome to the **Health Risk Prediction** project! This repository contains an end-to-end machine learning solution that predicts an individual's health condition using lifestyle, wellness, and physiological indicators.

The model classifies individuals into:

✅ Fit

⚠️ At-Risk

🚨 Unhealthy

using advanced data preprocessing, feature engineering, and CatBoost Classification.

---

# 🚀 Project Overview

Healthcare organizations collect large amounts of wellness and lifestyle data. Identifying health risks early can help individuals improve their quality of life and prevent future health complications.

This project analyzes factors such as:

- Sleep Duration
- Heart Rate
- BMI
- Stress Level
- Physical Activity
- Exercise Duration
- Water Intake
- Diet Type
- Smoking & Alcohol Habits
- Sleep Quality

and predicts an individual's overall health condition.

---

# 📊 Dataset Information

Dataset Characteristics:

- Records: **93,300+**
- Features: **20**
- Target Variable: **Health Condition**

Target Classes:

```text
Fit
At-Risk
Unhealthy
```

---

# 📖 Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/akkikoomar27/health-risk-prediction-catboost.git

cd health-risk-prediction-catboost
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

Open:

```text
Predicting_Student_Health_Risk.ipynb
```

in Google Colab, Jupyter Notebook, or VS Code.

---

# 🔍 Exploratory Data Analysis

Performed:

- Missing Value Analysis
- Duplicate Record Detection
- Numerical Feature Analysis
- Categorical Feature Analysis
- Outlier Detection
- Target Variable Analysis
- Health Risk Relationship Analysis

### Key Findings

- Stress Level significantly impacts health condition.
- Sleep Duration is one of the strongest predictive variables.
- Active individuals tend to have healthier outcomes.
- BMI and Heart Rate contribute strongly to risk classification.
- Poor sleep quality increases health risk probability.

---

# ⚙️ Feature Engineering

Custom healthcare features were created to improve model performance.

### BMI Category

```text
Underweight
Normal
Overweight
Obese
```

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

# 🤖 Machine Learning Model

Algorithm Used:

```text
CatBoost Classifier
```

Model Parameters:

```python
iterations = 300
learning_rate = 0.1
depth = 6
loss_function = "MultiClass"
eval_metric = "TotalF1"
```

---

# 📈 Results

| Metric | Value |
|----------|----------|
| Dataset Size | 93,300+ Records |
| Algorithm | CatBoost Classifier |
| Classes | 3 |
| Best Iteration | 266 |
| Validation F1 Score | 96.74% |

### Prediction Distribution

```text
At-Risk      : 122,302
Unhealthy    : 9,402
Fit          : 7,139
```

---

# 📊 Feature Importance

Top influential features identified by CatBoost:

- Stress Level
- Sleep Duration
- Physical Activity Level
- BMI
- Heart Rate
- Smoking & Alcohol Habits

These factors played a major role in determining an individual's health risk classification.

---

# 📸 Project Outputs

## Model Training Performance

Upload: `06_model_training.png`

## Feature Importance Analysis

Upload: `07_feature_importance.png`

## Prediction Output

Upload: `08_prediction_output.png`

## Submission Distribution

Upload: `09_submission_distribution.png`

---

# 🎯 Features

- End-to-End Machine Learning Workflow
- Data Cleaning & Preprocessing
- Missing Value Handling
- Exploratory Data Analysis (EDA)
- Feature Engineering
- CatBoost Multiclass Classification
- Feature Importance Analysis
- Health Risk Prediction
- Prediction Export to CSV

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- CatBoost
- Google Colab

---

# 📂 Project Structure

```text
health-risk-prediction-catboost/

│
├── README.md
├── Predicting_Student_Health_Risk.ipynb
├── sample_submission.csv
├── test.csv
│
└── screenshots/
    ├── 06_model_training.png
    ├── 07_feature_importance.png
    ├── 08_prediction_output.png
    └── 09_submission_distribution.png
```

---

# 📚 Notebook

- Predicting_Student_Health_Risk.ipynb

---

# 👨‍💻 Author

**Akhilesh Yadav**

Data Analyst | Data Scientist

### Skills

- Python
- SQL
- Power BI
- Machine Learning
- Snowflake
- SSIS
- Azure SQL

GitHub:
https://github.com/akkikoomar27

---

⭐ If you found this project useful, consider giving it a star!
