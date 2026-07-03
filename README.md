# 💳 Credit Card Approval Prediction System

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Web%20Framework-red.svg)](https://flask.palletsprojects.com/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-AI--Predictive-orange.svg)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Banks and financial institutions process thousands of credit card applications daily. Evaluating these requests manually is highly time-consuming, prone to human error, and inefficient at scale. Common grounds for immediate rejection include heavy outstanding loan balances, insufficient verifiable income, or excessive recent credit inquiries.

This project **automates the credit card approval pipeline** using AI/ML classification algorithms. By training predictive engines on structured historical applicant demographics and repayment behavior data, the system outputs immediate approval or rejection decisions—simulating exact real-world banking logic.

---

## 🚀 Key Features

* **Multi-Algorithm Engine:** Implements and evaluates four robust classification models: **Logistic Regression, Random Forest, XGBoost (Gradient Boosting), and Decision Trees**.
* **Feature Engineering Pipeline:** Custom pre-processing scripts compress multi-class past-due loan status records into strict binary risk labels.
* **Interactive Frontend UI:** Built natively on a lightweight **Flask backend** allowing internal bank credit analysts or external clients to interface directly with predictive instances.
* **Production Deployment:** Integrates with an **IBM Watson Machine Learning** delivery pipeline, creating cloud-hosted endpoints ready to serve scalable, real-time predictions.

---

## 💡 System Workflows & Supported Scenarios

### Scenario 1: Automated Credit Card Application Screening
A bank credit analyst registers an applicant's complete financial profile (e.g., income class, employment tenure, and credit history metrics). The system generates an immediate prediction response, highlighting marginal cases that require manual intervention.

### Scenario 2: High-Risk Applicant Identification & Compliance Review
Compliance staff deploy batch screening routines to evaluate applicants with unstable past due data fields. The underlying model automatically segregates high-risk profiles based on engineered financial risk markers.

### Scenario 4: Customer Self-Service Credit Card Eligibility Check
Prospective clients interact directly with a public facing interface to test their personal baseline parameters prior to logging a formal inquiry, mitigating unnecessary hard credit inquiries.

---

## 💻 Tech Stack

* **Programming Language:** Python
* **Web Architecture:** Flask (WSGI Web App Engine)
* **AI/Machine Learning:** Scikit-Learn, XGBoost, Pandas, NumPy
* **Infrastructure & MLOps:** IBM Watson Machine Learning, Cloud Object Storage
* **Database Management:** Relational Schema (SQL Architecture) — *[See DATABASE.md](./DATABASE.md) for full structural mappings.*

---

## 🔧 Local Installation & Setup

### 1. Clone the Workspace
```bash
git clone [https://github.com/yourusername/credit-card-approval-prediction.git](https://github.com/yourusername/credit-card-approval-prediction.git)
cd credit-card-approval-prediction
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
pip install -r requirements.txt
FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your_secure_session_key
WATSON_API_KEY=your_ibm_watson_token_here
WATSON_URL=your_ibm_watson_endpoint_url
flask run
