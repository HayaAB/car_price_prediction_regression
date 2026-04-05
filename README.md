# 🚗 Car Price Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting used car prices using Machine Learning techniques.  
The main goal is to build accurate regression models that estimate car prices based on various vehicle features such as year, engine size, mileage, fuel type, and transmission.

The project demonstrates the **complete Machine Learning workflow**, including:

- Data cleaning
- Feature engineering
- Model training
- Model evaluation
- Cross-validation
- Hyperparameter tuning

---

## 🎯 Project Objectives

- Understand and explore real-world structured data
- Handle missing values and inconsistent data
- Convert categorical features into numerical format
- Train regression models to predict car prices
- Evaluate model performance using multiple metrics
- Improve model accuracy using Cross-Validation and Hyperparameter Tuning
- Identify the most important features affecting car prices

---

## 📂 Dataset Information

Dataset: **Car Price Prediction Dataset**

The dataset contains information about used cars, including:

- `name`
- `year`
- `selling_price` (Target Variable)
- `km_driven`
- `fuel`
- `seller_type`
- `transmission`
- `owner`
- `mileage`
- `engine`
- `max_power`
- `seats`

Source: Kaggle – Car Price Prediction Dataset

Total Records: **8,128 cars**

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Removed unnecessary columns (e.g., car name)
- Cleaned numeric columns (removed units such as "bhp")
- Handled missing values using median replacement
- Converted categorical variables using **One-Hot Encoding**
- Split dataset into:
  - Training Set (80%)
  - Testing Set (20%)
- Applied **StandardScaler** for feature scaling (when required)

---

## 📊 Exploratory Data Analysis (EDA)

EDA was performed to:

- Understand dataset structure
- Identify missing values
- Analyze feature distributions
- Explore relationships between features
- Prepare data for modeling

Common EDA steps included:

- `df.head()`
- `df.info()`
- `df.describe()`
- Missing value analysis
- Feature visualization

---

## 🤖 Models Implemented

### 1️⃣ Linear Regression

Used as a baseline regression model.

Evaluation Metrics:

- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- R² Score

This model provided an initial understanding of linear relationships between features and car prices.

---

### 2️⃣ Random Forest Regressor

Used to improve prediction accuracy using ensemble learning.

Random Forest significantly improved performance compared to Linear Regression.

Evaluation Metrics:

- MAE
- MSE
- R² Score

Feature importance was extracted to identify key predictors.

---

## 🔁 Cross-Validation

To ensure model reliability, **5-Fold Cross Validation** was applied.

Method used:

- `cross_val_score()`
- Metric: **R² Score**

Result:

The model showed consistent performance across folds, indicating stable learning and minimal overfitting.

---

## ⚙️ Hyperparameter Tuning

Hyperparameter tuning was performed using:

**GridSearchCV**

Parameters tuned:

- `n_estimators`
- `max_depth`
- `min_samples_split`

Best Parameters Found:

```python
{
 'max_depth': 20,
 'min_samples_split': 2,
 'n_estimators': 100
}

----

## 📊 Feature Importance Analysis

The most influential features in predicting car prices were:

1. max_power
2. year
3. km_driven
4. engine
5. mileage

This indicates that engine performance and vehicle age are major factors affecting car prices.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🎯 Project Outcome

A high-performance machine learning model was successfully developed to predict used car prices with strong accuracy.

This project demonstrates the complete machine learning workflow, including:

- Data cleaning
- Feature engineering
- Model training
- Model evaluation
- Performance comparison
- Feature importance analysis

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Cross-validation
- Model deployment using Flask or Streamlit
- Building an interactive prediction interface
