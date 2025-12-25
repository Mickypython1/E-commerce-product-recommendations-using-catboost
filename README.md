# E-commerce-product-recommendations-using-catboost
# Overview
This project implements a product recommendation system for an e-commerce platform using the CatBoost algorithm. The goal is to predict items a customer is likely to be interested in based on their browsing and purchase history, thereby enhancing customer experience and increasing sales.

# Features
Handles categorical data and missing values efficiently with CatBoost.

Implements RFM (Recency, Frequency, Monetary) feature engineering.

Splits data into train/test sets for evaluation.

Provides feature importance visualization to understand model behavior.

Interactive GUI with ipywidgets for real-time recommendations.

# Implementation Steps
1. Import Libraries
NumPy, Pandas, Matplotlib, Seaborn

scikit-learn for preprocessing and evaluation

CatBoost for modeling

ipywidgets for interactive GUI

# 2. Load Dataset
Uses the Online Retail dataset.

Cleans missing values and filters invalid entries.

# 3. Data Preprocessing
Convert InvoiceDate to datetime.

Create TotalPrice column (Quantity × UnitPrice).

Remove negative quantities.

# 4. Feature Engineering
Compute RFM metrics per customer:

Recency → Days since last purchase

Frequency → Number of unique invoices

Monetary → Total spending

# 5. Train-Test Split
80% training, 20% testing.

Target variable: 1 if Monetary > median, else 0.

# 6. Train CatBoost Model
Parameters: iterations=100, learning_rate=0.1, depth=6.

Achieves high accuracy (initially overfitted, tuned further).

# 7. Feature Importance
Visualizes contribution of Recency, Frequency, and Monetary.

Identifies Monetary as dominant feature.

# 8. Interactive GUI
Sliders for Recency, Frequency, and Monetary.

Real-time prediction: Recommend or Do not recommend.
