# IBM Stock Trend-Regime Prediction using Machine Learning

This repository contains the source code and notebooks for an MSc Data Science project focused on short-horizon stock trend classification using historical market data for IBM.

The project formulates stock price prediction as a supervised classification problem, where market conditions are classified into uptrend and downtrend regimes rather than forecasting exact future prices. This approach improves stability and interpretability when modelling noisy financial time-series data.

# The workflow follows industry best practices and includes:

Data collection and preprocessing of historical OHLCV stock data

Feature engineering using technical indicators, momentum, and volume-based features

Time-aware train–validation–test splitting to prevent information leakage

Implementation and comparison of multiple machine learning models

Hyperparameter tuning and performance evaluation using standard classification metrics

Feature importance analysis to assess the contribution of different feature groups

# Models Implemented

Logistic Regression (baseline linear model)

Random Forest Classifier (ensemble bagging approach)

XGBoost Classifier (gradient boosting method)

# Evaluation Metrics

Models are evaluated using Accuracy, Precision, Recall, and F1-score, with particular emphasis on Recall and F1-score for reliable trend-regime identification.

# Tools & Technologies

Python (Pandas, NumPy, Scikit-learn, XGBoost)

Jupyter Notebooks

Matplotlib & Seaborn for visualisation

# Project Structure

The repository is organised into clearly defined folders for data, notebooks, source code, trained models, and reports to ensure reproducibility and clarity.

# Objective

The primary objective of this project is to assess the effectiveness of machine learning models in identifying short-term market trends and to analyse which types of features contribute most to predictive performance.

# Disclaimer

This project is intended for academic and research purposes only and does not constitute financial or investment advice.
