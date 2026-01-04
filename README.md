Budget Overrun Prediction in Construction Projects using Machine Learning
Project Overview

Budget overruns remain a critical challenge in construction projects, often leading to financial losses, project delays, and reduced stakeholder confidence. Traditional cost estimation methods rely heavily on expert judgement and static assumptions, which limits their ability to capture complex, non-linear relationships between project characteristics and costs.

This project applies machine learning techniques to predict budget overruns in construction projects using real-world regulatory data. The objective is to support early cost-risk identification and enable data-driven decision-making in construction project management.

🎯 Objectives

Formulate budget overrun prediction as a supervised classification problem

Perform robust data preprocessing and feature engineering

Train and compare multiple machine learning models

Identify the most effective model for predicting budget overruns

Analyse the contribution of different feature groups to model performance

🗂 Dataset

Source: Gujarat Real Estate Regulatory Authority (RERA), India

Access Link:
https://www.kaggle.com/datasets/ethon0426/gujarat-real-estate-project-registered-2017-2022

Records: 14,507 construction projects

Features: 44 attributes (categorical, numerical, administrative)

Dataset Highlights

Project characteristics (type, promoter, redevelopment status)

Cost-related variables (estimated cost, received amount, land cost)

Area and scale metrics (built-up area, carpet area, land area)

Regulatory and administrative project information

The dataset is publicly available, collected for regulatory transparency, and contains no personal or sensitive data.

🧠 Problem Formulation

Task: Binary classification

Target Variable: budget_overrun

1 → Project incurred cost exceeds estimated cost

0 → Project remains within budget

This formulation enables the application of machine learning models to predict cost-risk outcomes rather than exact cost values.

⚙️ Methodology
1️⃣ Data Preprocessing

Data cleaning and formatting

Handling missing values introduced by rolling calculations

Categorical encoding

Feature scaling using standardisation

Time-aware train–validation–test split

2️⃣ Feature Engineering

Cost and financial indicators

Area and scale-related features

Project characteristic variables

Removal of non-informative administrative fields

3️⃣ Machine Learning Models

The following classification models were implemented and evaluated:

Logistic Regression

K-Nearest Neighbours (KNN)

Decision Tree

Neural Network

Gradient Boosting Classifier

4️⃣ Evaluation Metrics

Models were evaluated using:

Accuracy

Precision

Recall

F1-score

🏆 Key Results

All machine learning models performed better than a random baseline

Gradient Boosting Classifier achieved the strongest overall performance

Cost-related, area-based, and scale features were the most influential predictors

Results confirm that machine learning can effectively capture budget overrun risk patterns

📈 Technologies Used

Programming Language: Python

Libraries:

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Environment: Jupyter Notebook

📁 Repository Structure
├── data/
│   └── gujarat_rera_projects.csv
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_model_evaluation.ipynb
├── results/
│   ├── evaluation_metrics.csv
│   └── feature_importance.png
├── README.md
└── requirements.txt

🚀 How to Run the Project

Clone the repository:

git clone https://github.com/your-username/budget-overrun-prediction.git


Install dependencies:

pip install -r requirements.txt


Run the notebooks in order:

01_data_preprocessing.ipynb

02_feature_engineering.ipynb

03_model_training.ipynb

04_model_evaluation.ipynb

⚠️ Limitations

Analysis is limited to a single geographic region (Gujarat, India)

Does not include macroeconomic or sentiment-based variables

Transaction costs and real-world execution constraints are not modelled

🔮 Future Work

Extend the framework to multiple regions and countries

Integrate macroeconomic and market indicators

Incorporate text-based sentiment analysis from news sources

Apply advanced deep learning models such as LSTM

Perform cost-sensitive learning and backtesting

📜 Ethical Considerations

The dataset is publicly available and contains no personal or sensitive information. All analysis complies with ethical research practices and data protection principles.
