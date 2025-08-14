# Ford PriceSense : Used Car Price Prediction
![Python](https://img.shields.io/badge/Python-3.9-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-ScikitLearn-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## Project Overview
**Ford PriceSense** is a machine learning project developed for a used car dealership specializing in Ford vehicles.  
The objective is to **predict the optimal selling price** for cars in the dealer's inventory based on historical sales data.  

The project uses a publicly available dataset from Kaggle (slightly modified) containing detailed information on Ford car sales, including attributes such as model, year, transmission type, mileage, fuel type, tax, mpg, engine size, and price.

This project involves:
- Data cleaning & preprocessing
- Exploratory data analysis (EDA)
- Single-variable and multi-variable regression modeling
- Model performance comparison (Linear, Polynomial, Ridge)
- Hyperparameter tuning using Grid Search
- Final model selection for optimal predictions

---

## Project Steps

### 1️. Data Cleaning
- Removed duplicate entries.
- Handled missing values.
- Ensured correct data types for each column.

### 2️. Exploratory Data Analysis
- Counted sales for each **fuel type**.
- Identified **transmission type** with the most price outliers.
- Visualized relationships between variables and price.

### 3️. Feature Engineering
- Separated **numeric** and **categorical** features.
- Applied **StandardScaler** to numeric features.
- Applied **OneHotEncoding** to categorical features.

### 4️. Modeling
**Single-variable regressions:**
- Linear Regression
- Polynomial Regression (degree 2 & 3)
- Ridge Regression

**Multi-variable regressions:**
- Linear Regression
- Polynomial Regression (degree 2)
- Ridge Regression (baseline)
- Ridge Regression with Grid Search hyperparameter tuning

### 5️. Model Selection
- Evaluated models using **RMSE** and **R²** on a hold-out test set.
- Selected the best Ridge Regression model from Grid Search as the final predictor.

---

## 🔍 Results Summary

<img width="693" height="174" alt="image" src="https://github.com/user-attachments/assets/b050907c-e3f4-4605-b0b4-f70b7e9e0bdd" />

---

## Key Insights
- Certain fuel types dominate sales volume.
- Transmission type has a strong influence on price variability.
- Ridge Regression with tuned hyperparameters consistently outperforms other models in predictive accuracy.
<img width="1780" height="686" alt="image" src="https://github.com/user-attachments/assets/4c1b2c46-65f7-476d-8759-fa5f6876853d" />


---

**💡 Contributions, suggestions, and improvements are welcome! Fork the repo and submit a pull request.**
