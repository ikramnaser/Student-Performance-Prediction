# 🎓 Student Performance Prediction with Multiple Linear Regression

This project applies **Multiple Linear Regression** to predict student academic performance based on various behavioral and academic factors. The dataset includes 10,000 students and explores how elements like study habits, sleep, and extracurricular activities influence their performance.

---

## 📌 Project Objectives

- Explore and visualize patterns in student performance data.
- Build a predictive model using **Multiple Linear Regression**.
- Evaluate model performance using appropriate metrics.
- Derive a regression equation to interpret the impact of each variable.

---

## 📁 Dataset Overview

The dataset includes the following features:

| Feature                             | Description                                      |
|-------------------------------------|--------------------------------------------------|
| `Hours Studied`                     | Daily study time in hours                       |
| `Previous Scores`                   | Past academic scores (percentage)               |
| `Extracurricular Activities`        | Participation in extracurriculars (`Yes`/`No`) |
| `Sleep Hours`                       | Daily sleep in hours                            |
| `Sample Question Papers Practiced` | Number of mock exams attempted                  |
| `Performance Index`                 | Target variable (performance score out of 100)  |

---

## 🔍 Exploratory Data Analysis

- **Correlation Analysis**: Strong positive correlations found between `Hours Studied`, `Previous Scores`, and the `Performance Index`.
- **Visualizations**:
  - Line plot of average performance by hours studied.
  - Regression plot between previous scores and performance.
  - Box plots comparing categorical and numerical features with performance.
  - Correlation heatmap.

---

## 🧹 Data Preprocessing

- **Train-Test Split**: 80% training, 20% testing.
- **Label Encoding**: Converted `Extracurricular Activities` from categorical to numeric (Yes = 1, No = 0).

---

## 🧠 Model Training

- Algorithm: `LinearRegression` from Scikit-learn.
- Trained the model on preprocessed features to predict `Performance Index`.

---

## 📈 Model Evaluation

- **R² Score (Train)**: `0.9887`
- **R² Score (Test)**: `0.9890`
- **Mean Squared Error**: `4.08`

The model demonstrates **excellent predictive performance**, suggesting that the selected features are highly informative.

---

## 📊 Regression Equation

The derived multiple linear regression equation is:
Performance Index =
2.85 × Hours Studied +
1.02 × Previous Scores +
0.61 × Extracurricular Activities (0 or 1) +
0.48 × Sleep Hours +
0.19 × Sample Question Papers Practiced
- 33.92

