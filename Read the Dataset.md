# 📖 Phase 1: Reading the Dataset

## Description
Reading the dataset is an important step in the Credit Card Approval Prediction project because it helps understand the structure, features, and records available for machine learning. 

The dataset is loaded using the Pandas library with functions such as `pd.read_csv()` to read CSV files and store them in a DataFrame for analysis and preprocessing. Functions like `head()`, `shape`, and `info()` are used to display sample records, dataset size, column names, data types, and missing values before model training.

---

## Code Implementation

In pandas, we have a function called `read_csv()` to read the dataset. As a parameter, we have to give the directory of the CSV file. For this project, we are loading two separate files: the application records and the credit history records.

```python
import pandas as pd

# Load the datasets into DataFrames
app = pd.read_csv('application_record.csv')
credit = pd.read_csv('credit_record.csv')
