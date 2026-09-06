# 🏠 House Price Prediction using Machine Learning

## 📌 Project Overview

This project predicts house prices using Machine Learning based on various property-related features.

The project follows a complete machine learning workflow including data exploration, preprocessing, feature engineering, outlier handling, categorical encoding, feature scaling, model training, and evaluation.

## 📊 Dataset

The dataset contains **4,600 house records** with features related to:

- Number of bedrooms
- Number of bathrooms
- Living area
- Lot area
- Floors
- Waterfront
- View
- Condition
- Basement area
- City
- Year built
- Renovation year
- House price

The dataset contains **18 original columns**. No duplicate or missing records were found during the initial data analysis. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

## 🔧 Data Preprocessing

The following preprocessing techniques were applied:

- Extracted year and month from the date column
- Removed unnecessary columns
- Created a `house_age` feature
- Removed selected features based on analysis
- Applied logarithmic transformation to the target price
- Handled outliers using the IQR method
- Encoded the categorical `city` feature using One-Hot Encoding
- Applied StandardScaler to features and target

## 🤖 Machine Learning Model

The project uses:

**Support Vector Regression (SVR)**

- Kernel: RBF
- Train-Test Split: 80:20
- Random State: 1

The SVR model was trained after feature encoding and standardization. :contentReference[oaicite:4]{index=4} :contentReference[oaicite:5]{index=5}

## 📈 Model Evaluation

The model achieved a **training R² score of approximately 0.77**.

> Note: This value represents the training-set R² score reported in the notebook and should not be interpreted as test accuracy. :contentReference[oaicite:6]{index=6}

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 🔄 Project Workflow

1. Data Loading
2. Exploratory Data Analysis
3. Data Cleaning
4. Feature Engineering
5. Outlier Detection and Removal
6. Categorical Feature Encoding
7. Feature Scaling
8. Train-Test Split
9. SVR Model Training
10. Model Evaluation

## 📁 Project Structure

```text
house-price-prediction/
│
├── house_prediction.ipynb
└── README.md
