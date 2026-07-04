# 🧩 Phase 3: Multivariate Analysis

## Description
Multivariate Analysis is performed to study the relationship and interaction between multiple features in the dataset at the same time. In the Credit Card Approval Prediction project, this analysis helps understand how different applicant attributes—such as income, employment days, family members, and age—are related to each other and how they influence the approval prediction process. 

This step is essential for identifying correlations, hidden patterns, and feature dependencies within the dataset.

### Key Techniques Used:
* **Correlation Analysis:** The `app.corr()` function calculates the correlation values between numerical features in the dataset.
* **Heatmaps:** We use Seaborn's heatmap functionality to graphically represent these feature relationships. The heatmap displays positive and negative correlations using different color gradients, making it easier to identify strongly related variables.

### Benefits for Machine Learning:
* Aids in **feature selection** by identifying the variables with the greatest impact on credit card approval.
* Helps **reduce redundancy** (e.g., if two features are highly correlated, one might be dropped to simplify the model).
* Improves overall **model performance and optimization**.

---

## Code Implementation

Below is the code used to generate the correlation heatmap for the numerical variables in our application dataset.

```python.
import matplotlib.pyplot as plt
import seaborn as sns

# Set the figure size for better readability
fig, ax = plt.subplots(figsize=(8,6))

# Generate the heatmap with annotations
# Ensure that 'app' only contains numeric columns before running corr()
# e.g., numeric_app = app.select_dtypes(include=['float64', 'int64'])
# sns.heatmap(numeric_app.corr(), annot=True)

sns.heatmap(app.corr(), annot=True)

# Display the plot
plt.show()
