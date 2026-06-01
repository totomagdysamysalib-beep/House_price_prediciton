# House Price Prediction - Regression Benchmarking

This repository contains a comprehensive comparison of 5 different Machine Learning regression models to predict house prices. 

## 📊 Project Overview
The goal of this project is to apply and benchmark various regression algorithms on the housing.csv dataset. Special attention was paid to machine learning best practices, such as preventing *Data Leakage* by fitting preprocessing transformers (Imputers, Encoders, and Scalers) strictly on the training set.

## 🛠️ Data Preprocessing Pipeline
- *Missing Data:* Handled using SimpleImputer (mean strategy).
- *Categorical Variables:* Encoded using OneHotEncoder.
- *Feature Scaling:* Applied StandardScaler where required (e.g., SVR).

## 🚀 Models Implemented & Performance
Here is the performance summary of the models based on the *R² Score*:

| Model | R² Score |
| :--- | :--- |
| *Random Forest Regression* | *0.810* |
| *Support Vector Regression (SVR)* | *0.756* |
| *Polynomial Regression* | *0.692* |
| *Decision Tree Regression* | *0.642* |
| *Multiple Linear Regression* | *0.638* |

## 💡 Key Takeaways
- *Ensemble Methods Win:* Random Forest outperformed all other models, proving the power of combining multiple decision trees to reduce overfitting.
- *Non-linearity:* Models that handle non-linear relationships (SVR, Random Forest) performed significantly better than linear models.
