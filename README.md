# Predicting-Health-Insurance-Costs-Using-Machine-Learning
This project applies multiple machine learning models to predict individual health insurance charges based on demographic, lifestyle, and medical-related features.  
The goal is to explore feature impact (e.g., smoking, BMI), compare different regression models, and identify the best-performing approach through systematic evaluation.

## Project Overview

Health insurance costs vary significantly across individuals due to factors such as age, smoking habits, BMI, and medical history.  
In this project, I:

- Performed **data cleaning and preprocessing**
- Conducted **exploratory data analysis (EDA)**
- Trained and evaluated multiple **regression models**
- Compared models using standard performance metrics
- Saved the **best-performing model and preprocessing objects** for future inference

---

##  Dataset

- **Source**: Public medical insurance dataset
- **Target variable**: `charges`
- **Features include**:
  - `age`
  - `sex`
  - `bmi`
  - `children`
  - `smoker`
  - `region`

---

## Data Preprocessing

- Handled categorical variables using **Label Encoding**
- Applied **Standard Scaling** to numerical features
- Performed train-test split to avoid data leakage
- Verified data types and removed potential inconsistencies

Saved preprocessing objects:
- `standard_scaler.pkl`
- `label_encoder_gender.pkl`
- `label_encoder_diabetic.pkl`

---

## 🤖 Models Trained

The following regression models were implemented and compared:

- **Linear Regression**
- **Polynomial Regression** (degree 2 & 3)
- **Ridge Regression**
- **Lasso Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

Each model was evaluated using the same train/test split for fair comparison.

---

##  Model Evaluation Metrics

Models were evaluated using:

- **R² Score**
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

The evaluation logic is encapsulated in a reusable function for consistency.

---

##  Best Model

After comparison, the **best-performing model** was selected based on test-set performance and saved for deployment or future inference: