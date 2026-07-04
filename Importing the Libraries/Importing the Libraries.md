# Credit Card Approval Prediction

## Project Overview
Banks and financial institutions receive thousands of credit card applications every day. A significant portion of these are rejected due to factors such as high existing loan balances, insufficient income levels, or excessive credit inquiries. Manually reviewing each application is both time-consuming and highly prone to human error, making it an inefficient process at scale.

This project automates the credit card approval decision using Machine Learning. By training a predictive model on historical applicant data, the system evaluates financial and demographic inputs to determine whether an applicant is likely to be approved or rejected, just as real banks do. 

The project evaluates four classification algorithms to find the best-performing model:
* Logistic Regression
* Random Forest
* XGBoost (Gradient Boosting)
* Decision Tree

---

## Step 1: Importing the Libraries

Importing the required libraries is the first fundamental step in the Credit Card Approval Prediction workflow. These libraries provide the necessary functions and modules for data analysis, preprocessing, visualization, machine learning model training, and performance evaluation. 

Key libraries utilized include:
* **Pandas & NumPy:** For robust data manipulation, handling dataframes, and numerical computations.
* **Matplotlib & Seaborn:** For exploratory data analysis (EDA) and visualizing data distributions.
* **Scikit-Learn (sklearn):** The core machine learning library used for splitting data, encoding categorical variables, evaluating metrics, and building the classification models.

### Code Implementation

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
#from imblearn.combine import SMOTETomek
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import train_test_split, RandomizedSearchCV
from sklearn.preprocessing import OneHotEncoder
from sklearn.metrics import classification_report,confusion_matrix,f1_score
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import GradientBoostingClassifier
from sklearn.tree import DecisionTreeClassifier
