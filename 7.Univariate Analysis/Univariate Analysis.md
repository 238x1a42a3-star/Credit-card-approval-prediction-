# 📊 Phase 2: Univariate Analysis

## Description
Univariate Analysis is performed to study and understand a single feature or variable in the dataset independently. In the Credit Card Approval Prediction project, univariate analysis helps identify the distribution, frequency, and patterns of applicant-related attributes such as occupation type, income category, education level, and family status. This analysis makes it easier to detect dominant categories, unusual values, and overall data behavior before model training.

In this phase, functions such as `value_counts()` are used to count the frequency of individual categories, while visualization libraries like Matplotlib and Seaborn are used to create bar charts, count plots, and histograms for better understanding of the data distribution. 

### Key Benefits:
* **Pattern Recognition:** Generated graphs and plots help in identifying trends, class imbalance, and feature importance within the dataset.
* **Better Preprocessing:** This analysis improves data understanding and supports better preprocessing, feature selection, and machine learning performance.

---

## Code Implementation

For example, we use `app['OCCUPATION_TYPE'].value_counts()` to display the number of applicants in each occupation category, and `sns.countplot()` to visualize the distribution graphically.

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Print the text summary of occupation counts
print("Number of people working status :")
print(app['OCCUPATION_TYPE'].value_counts())

# Set the figure size for the plot
sns.set(rc={'figure.figsize':(18,6)})

# Create a countplot to visualize the distribution
sns.countplot(x='OCCUPATION_TYPE', data=app, palette='Set2')

# Display the plot
plt.show()


7.Univariate Analysis.md
