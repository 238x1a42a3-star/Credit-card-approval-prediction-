# Task 2 – Pre-requisites (Tools & Technologies)

## Project Name

**Credit Card Approval Prediction Using Machine Learning**

---

# Objective

The objective of this task is to install and configure the required software, Python libraries, and development tools necessary for building the Credit Card Approval Prediction project. These tools enable data preprocessing, visualization, machine learning model development, and deployment through a web application.

---

# Introduction

The Credit Card Approval Prediction project is developed using Python and several open-source libraries that support data analysis, machine learning, visualization, and web application deployment. Before starting the project, it is essential to install all the required software and packages to ensure a smooth development process.

These tools provide an efficient environment for data processing, model training, evaluation, and real-time prediction.

---

# Software and Libraries Used

## 1. Anaconda Navigator

### Purpose
Anaconda Navigator is a graphical interface used to manage Python environments, install packages, and launch development tools such as Jupyter Notebook and Spyder.

### Features
* Environment Management
* Package Installation
* Jupyter Notebook Support
* Python Distribution

---

## 2. PyCharm

### Purpose
PyCharm is a professional Integrated Development Environment (IDE) used for writing, debugging, and executing Python programs.

### Features
* Intelligent Code Completion
* Integrated Debugger
* Project Management
* Git Integration
* Virtual Environment Support

---

## 3. NumPy

### Purpose
NumPy provides high-performance numerical computing capabilities using multidimensional arrays and mathematical operations.

### Applications in this Project
* Array Operations
* Numerical Calculations
* Matrix Computations
* Statistical Functions

---

## 4. Pandas

### Purpose
Pandas is used for loading, cleaning, manipulating, and analyzing datasets efficiently.

### Applications in this Project
* Reading CSV Files
* Handling Missing Values
* Data Cleaning
* Feature Selection
* Data Transformation

---

## 5. Scikit-learn

### Purpose
Scikit-learn provides machine learning algorithms used for classification, regression, preprocessing, and model evaluation.

### Algorithms Used
* Logistic Regression
* Decision Tree
* Random Forest

### Applications in this Project
* Model Training
* Data Splitting (Train/Test)
* Performance Evaluation
* Prediction Inference

---

## 6. Matplotlib

### Purpose
Matplotlib is a visualization library used for creating graphs and charts.

### Applications in this Project
* Histogram
* Bar Chart
* Pie Chart
* Scatter Plot
* Line Graph

---

## 7. Seaborn

### Purpose
Seaborn is built on top of Matplotlib and provides attractive statistical visualizations.

### Applications in this Project
* Heatmaps
* Correlation Matrix
* Count Plots
* Box Plots
* Distribution Plots

---

## 8. Flask

### Purpose
Flask is a lightweight web framework used for deploying the trained machine learning model as a web application.

### Applications in this Project
* Web Application Development
* Prediction API
* HTML Integration
* Model Deployment

---

## 9. XGBoost

### Purpose
XGBoost is an optimized distributed gradient boosting library designed to be highly efficient, flexible, and portable.

### Applications in this Project
* Gradient Boosting Classification Model Training
* High-Accuracy Performance Comparison

---

# Development Workflow

1. **Install Anaconda Navigator:** Download and install Anaconda to manage the system environment.
2. **Create a Python Virtual Environment:** Isolate project package dependencies.
3. **Install Required Python Libraries:** Set up the modeling and server utilities.
4. **Develop and Test Machine Learning Models:** Execute data loading, preprocessing, training, and evaluation in PyCharm or Jupyter Notebook.
5. **Build the Flask Web Application:** Construct routing, templates, and backend inference handlers.
6. **Deploy the Trained Model:** Load the saved binary model inside the web app for real-time predictions.

---

# Required Python Packages

Install the required libraries using the following command in your terminal:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn flask xgboost
```

---

# Technologies Summary

| Tool / Library | Purpose |
| :--- | :--- |
| **Anaconda Navigator** | Python Environment Management |
| **PyCharm** | Python IDE |
| **NumPy** | Numerical Computing |
| **Pandas** | Data Processing |
| **Scikit-learn** | Machine Learning |
| **Matplotlib** | Data Visualization |
| **Seaborn** | Statistical Visualization |
| **Flask** | Web Application Development |
| **XGBoost** | Gradient Boosting Model |

---

# Environment & Technology Stack Diagram

```mermaid
graph TD
    subgraph "Development Environment"
        Anaconda["Anaconda Navigator <br> (Environment Manager)"]
        PyCharm["PyCharm Community IDE <br> (Code Editor & Debugger)"]
    end
    
    subgraph "Python Virtual Environment (.venv)"
        Packages["Required Packages"]
        
        subgraph "Data Science & Visualization"
            NumPy["NumPy <br> (Array Computations)"]
            Pandas["Pandas <br> (Data Processing)"]
            Matplotlib["Matplotlib <br> (Plotting Engine)"]
            Seaborn["Seaborn <br> (Statistical Plots)"]
        end
        
        subgraph "Machine Learning Modeling"
            ScikitLearn["Scikit-learn <br> (Logistic Regression, Decision Tree, Random Forest)"]
            XGBoost["XGBoost <br> (Gradient Boosting Classifier)"]
        end
        
        subgraph "Web Application & Deployment"
            Flask["Flask <br> (Lightweight Web Server)"]
        end
    end
    
    Anaconda -->|.venv creation| Packages
    PyCharm -->|Code Execution| Packages
    Packages --> Data Science & Visualization
    Packages --> Machine Learning Modeling
    Packages --> Web Application & Deployment
    
    style Anaconda fill:#dfd,stroke:#333
    style PyCharm fill:#dff,stroke:#333
    style NumPy fill:#ffd,stroke:#333
    style Pandas fill:#ffd,stroke:#333
    style ScikitLearn fill:#fdf,stroke:#333
    style XGBoost fill:#fdf,stroke:#333
    style Flask fill:#fdd,stroke:#333
```

---

# Expected Outcome

After completing the pre-requisites:
- All required software is installed successfully.
- Python development environment is configured.
- Machine learning libraries are ready for use.
- Flask framework is available for application development.
- The system is prepared for dataset preprocessing, model training, and deployment.

---

# Conclusion

The successful installation and configuration of the required tools establish the development environment for the Credit Card Approval Prediction project. These technologies support efficient data analysis, machine learning model development, visualization, and deployment, enabling the creation of a reliable and scalable prediction system.
