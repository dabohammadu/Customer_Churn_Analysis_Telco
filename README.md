# Customer_Churn_Analysis_Telco

Machine learning project that predicts bank customer churn using Python and Scikit-learn, covering EDA, feature engineering, model comparison, and deployment-ready pipelines.

This project builds an end-to-end machine learning pipeline in Python to predict customer churn using bank customer data. The goal is to identify customers likely to leave so businesses can take proactive steps to improve customer retention and lifetime value.

The project demonstrates the complete data science workflow, including data exploration, feature engineering, model training, evaluation, and deployment-ready pipelines.

Project Workflow

The machine learning pipeline includes:

Data Loading and Inspection

Exploratory Data Analysis (EDA)

Feature Engineering

Data Preprocessing (Encoding & Scaling)

Train/Test Split

Model Training and Cross Validation

Model Evaluation

Feature Importance Analysis

Model Saving for Deployment

Dataset

The dataset contains banking customer information used to predict churn.

Key features include:

Credit Score

Country

Gender

Age

Tenure

Account Balance

Number of Products

Credit Card Ownership

Active Membership

Estimated Salary

Target variable:

Churn (1 = customer left, 0 = customer retained)

Exploratory Data Analysis

EDA was conducted to identify churn patterns using visualizations such as:

Distribution plots

Correlation heatmaps

Country and gender churn analysis

Product usage vs churn

Age and tenure analysis

Libraries used: Matplotlib and Seaborn

Feature Engineering

Additional features were created to capture financial behavior:

Balance per Product

Salary to Balance Ratio

These features help improve predictive performance.

Machine Learning Models

Multiple models were trained and compared using cross-validated ROC-AUC:

Logistic Regression

Random Forest

Gradient Boosting

AdaBoost

Evaluation metrics include:

Accuracy

Precision

Recall

F1 Score

ROC-AUC

Model Deployment

The final trained pipeline is saved using Joblib for future deployment:

joblib.dump(best_pipeline, "best_churn_pipeline.pkl")

This allows the model to be reused for production prediction systems or APIs.

Tools & Technologies

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Joblib

Business Impact

Churn prediction helps organizations:

Identify customers at risk of leaving

Improve retention strategies

Increase customer lifetime value

Optimize marketing efforts

Future Improvements

Possible enhancements include:

Hyperparameter tuning

XGBoost or LightGBM models

SHAP explainability

Streamlit dashboard

API deployment for real-time predictions
