# Telecom-Churning-Forecast---Project-16

# Telecom Churn Forecasting Project

## Project Overview
The goal of this project was to forecast customer churn for a telecom operator, **Interconnect**. Churn prediction is critical for customer retention, as it allows the business to proactively target at-risk customers. This project involved cleaning, preprocessing, feature engineering, and training various machine learning models to predict customer churn. The models were evaluated using the **AUC-ROC** score, with the final solution being an ensemble model that combined several individual models to improve performance.

## Project Structure
This repository contains the following files:



- **datasets/**:
    - `contract.csv`: Contains customer contract details, such as `customerID`, `BeginDate`, `EndDate`, `ContractType`, and other related information.
    - `personal.csv`: Contains customer demographic information, such as `customerID`, `Gender`, `Partner`, `Dependents`, etc.
    - `internet.csv`: Contains data about the customer’s internet services, including whether they have services such as `OnlineSecurity`, `OnlineBackup`, `TechSupport`, and `StreamingTV`.
    - `phone.csv`: Contains data about phone services, including whether the customer has `MultipleLines`.

- **notebooks/**:
    - `churn_prediction.ipynb`: This notebook contains the entire workflow of the project. It covers:
        - Data loading and exploration.
        - Data cleaning and preprocessing.
        - Feature engineering (creating new features like `ContractDuration`, `TotalServices`, etc.).
        - Handling class imbalance using **SMOTE**.
        - Model training, hyperparameter tuning, and evaluation (using Logistic Regression, Random Forest, XGBoost, LightGBM, and an Ensemble Model).
        - Evaluation of models using AUC-ROC and accuracy metrics.

- **models/**:
    - (Optional) This folder can be used to save trained models for future use or deployment (e.g., saving the ensemble model as `model.pkl`).
    

## How to Use the Project

### Steps to Run the Project
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/mattfuller2/telecom-churn-forecasting.git
2. Install the required dependencies:
   pip install -r requirements
3. Open Jupyter Notebook
   jupyter notebook
