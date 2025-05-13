
# Project Summary
This project predicts whether a customer is likely to churn (stop using a service). Churn prediction is important for companies like telecom providers or subscription services because retaining existing customers is cheaper than acquiring new ones.

In this project, I used a real-world customer dataset to train different machine learning models that classify customers as likely to churn or stay. I tried multiple models including Decision Tree, Random Forest, and XGBoost and compared their performance.


# Tools and Libraries Used
Python
Pandas & NumPy (for data manipulation)
Matplotlib & Seaborn (for visualization)
Scikit-learn (for machine learning models and metrics)
XGBoost (for gradient boosting model)

# Dataset Info
The dataset contains customer information such as:
Gender, Senior Citizen, Partner, Dependents
Phone and internet services
Contract type (Monthly, Yearly, etc.)
Payment method
Tenure, Monthly charges, Total charges
Target label: Churn (Yes/No)

# Project Workflow
**1. Data Exploration**
Loaded the dataset and viewed column names and sample rows.

Checked for missing or unusual values.

**2. Data Cleaning**
Dropped unnecessary columns like customerID.

Fixed missing values in TotalCharges by converting to numeric.

Converted Churn and other categorical columns to numerical values using LabelEncoder.

**3. Exploratory Data Analysis (EDA)**
Visualized distributions of important features using histograms and countplots.

Identified patterns like customers with month-to-month contracts being more likely to churn.

**4. Feature Selection and Preprocessing**
Selected important features for model training.

Encoded categorical features and scaled the data using StandardScaler.

**5. Model Building**
Trained the following models:
Decision Tree Classifier
Random Forest Classifier
XGBoost Classifier

**6. Model Evaluation**
Used accuracy score, confusion matrix, and classification report to evaluate performance.
Compared accuracy of all three models.


# Results
| Model         | Accuracy |
| ------------- | -------- |
| Decision Tree | \~78%    |
| Random Forest | \~80%    |
| XGBoost       | \~81%    |

XGBoost performed the best in this case.

**Customers with monthly contracts and electronic checks had higher churn risk.**


# What I Learned
How to clean and prepare real-world data for ML
How to use label encoding and feature scaling
How to train and compare multiple ML models
How to evaluate classification performance using metrics like confusion matrix
