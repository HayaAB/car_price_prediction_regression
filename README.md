# 🚗 Car Price Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on building a machine learning model to predict used car prices based on various features such as year, fuel type, engine power, and kilometers driven.

The objective was to develop an accurate regression model that can estimate car prices using real-world data from Kaggle.

---

## 📊 Dataset

- Source: Kaggle – Car Price Prediction Dataset
- Total Records: 8,128 cars
- Features included:
  - Year
  - Selling Price
  - Kilometers Driven
  - Fuel Type
  - Seller Type
  - Transmission
  - Owner
  - Mileage
  - Engine
  - Max Power
  - Seats

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Handling missing values
- Cleaning text values (removing units such as 'bhp')
- Converting string values to numeric format
- Encoding categorical features using One-Hot Encoding
- Feature scaling using StandardScaler
- Splitting data into training and testing sets

---

## 🤖 Models Used

Two regression models were implemented:

1. Linear Regression  
2. Random Forest Regressor

---

## 📈 Model Performance

### Linear Regression

- MAE: 268,886
- R² Score: 0.697

### Random Forest (Final Model)

- MAE: 70,122
- R² Score: **0.968**

Random Forest significantly improved prediction accuracy and became the final selected model.

---

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
