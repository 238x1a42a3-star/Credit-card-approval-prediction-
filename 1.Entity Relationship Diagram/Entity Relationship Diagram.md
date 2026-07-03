# Credit Card Approval Prediction using AI & Machine Learning

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Machine_Learning-Scikit--Learn-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 📌 Project Overview
A significant portion of financial institutions' revenue comes from credit cards, but managing default risks is a critical challenge. This project leverages **Artificial Intelligence and Machine Learning** to automate the credit card approval process. By analyzing historical applicant data (e.g., income, employment duration, debt, and credit history), the system predicts whether an applicant is a "good" or "bad" credit risk, minimizing human bias and accelerating decision-making.

## 📊 Dataset Description
The dataset used for this project typically contains two main sources of information (e.g., from the popular Kaggle Credit Card Approval dataset):
1. **Application Record (`application_record.csv`)**: Contains demographic and financial details of the applicants (Gender, Income, Education, Employment status, etc.).
2. **Credit Record (`credit_record.csv`)**: Contains historical payment data for the applicants, which is used to derive the target label (`Approved` / `Rejected` or `Good` / `Bad` client) using a vintage analysis approach.

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Libraries for Data Processing:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, XGBoost / LightGBM (optional)
* **Environment:** Jupyter Notebook / Google Colab

## 🚀 Key Features
* **Data Preprocessing & Cleaning:** Handling missing values, removing duplicates, and parsing data types.
* **Feature Engineering:** Balancing highly skewed datasets, encoding categorical variables (One-Hot / Label Encoding), scaling numerical features, and creating a target variable based on payment history.
* **Handling Class Imbalance:** Utilizing techniques like SMOTE (Synthetic Minority Over-sampling Technique) to address heavily imbalanced data.
* **Model Evaluation:** Comparing multiple algorithms (Logistic Regression, Decision Trees, Random Forest, XGBoost) using metrics like Accuracy, Precision, Recall, F1-Score, and ROC-AUC.

## 📂 Project Structure
```text
├── data/                  # Raw and processed datasets (Git-ignored if too large)
├── notebooks/             # Jupyter notebooks for EDA and model building
│   └── credit_card_approval.ipynb
├── src/                   # Python scripts for production pipeline
│   ├── data_preprocessing.py
│   └── train_model.py
├── models/                # Saved/serialized trained models (.pkl or .joblib)
├── README.md              # Project documentation
└── requirements.txt       # List of dependencies
