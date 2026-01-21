**Customer Churn Prediction & Retention Analysis System**

**1.Introduction**

Customer churn refers to the situation where customers stop using a company’s product or service. In competitive Telecom and SaaS industries, customer retention is crucial for maintaining revenue and long-term growth. Predicting churn in advance allows businesses to take proactive steps to retain customers.

This project focuses on building a Machine Learning–based system that predicts customer churn and identifies the key factors responsible for customer attrition. The project not only emphasizes prediction accuracy but also aims to generate meaningful business insights.

**2. Objective**

The main objectives of this project are:

* To predict whether a customer is likely to churn (Yes/No)

* To identify important factors contributing to customer churn

* To generate business-driven insights for customer retention strategies

* Recall and F1-score are treated as primary evaluation metrics due to class imbalance in churn data.

**3. Dataset Description**

The project uses a Telecom / SaaS Customer Churn dataset containing the following features:

* Customer tenure

* Monthly charges

* Total charges

* Contract type (Monthly / Yearly)

* Payment method

* Internet service type

* Customer support interactions

* Add-on services (OTT streaming, online security, cloud backup)

* Target variable: Churn (Yes / No)

* The dataset represents real-world customer behavior and is suitable for churn prediction analysis.

**4. Data Understanding and Cleaning**

The dataset was first explored to understand its structure, data types, and missing values.
Data cleaning steps included:

* Converting the TotalCharges column from string to numeric format

* Handling missing values using median imputation

* Verifying data consistency and completeness

* These steps ensured the dataset was clean and ready for analysis and modeling.

**5. Feature Engineering**

Feature engineering was performed to enhance model performance and extract meaningful insights. The following new features were created:

Average Monthly Spend: TotalCharges divided by tenure

Tenure Groups: Customers categorized as New, Mid, or Loyal

Service Usage Count: Total number of add-on services used by a customer

This step elevated the project from a basic ML implementation to an intermediate-level, industry-relevant solution.

**6. Exploratory Data Analysis (EDA)**

Exploratory Data Analysis was conducted to identify patterns and relationships related to customer churn. Key analyses included:

* Churn distribution across contract types

* Relationship between tenure and churn

* Monthly charges comparison between churned and retained customers

* Impact of customer support interactions on churn

* EDA results helped guide feature selection and model design decisions.

**7. Handling Imbalanced Data**

Customer churn datasets are typically imbalanced, with fewer churned customers compared to retained ones.
To address this issue:

* Class distribution was analyzed

* Class weights were applied during model training to balance the impact of churned customers

* This approach helped improve recall and overall model reliability.

**8. Model Building**

Multiple machine learning models were implemented and compared:

* Logistic Regression (Baseline model)

* Random Forest Classifier

* Feature scaling using StandardScaler was applied for Logistic Regression to ensure faster convergence and better performance.

**9. Model Evaluation**

Models were evaluated using the following metrics:

* Accuracy (secondary metric)

* Precision

* Recall (primary metric)

* F1-score

* Confusion Matrix

A comparison table was created to justify the selection of the final model based on performance.

**10. Model Interpretation**

To understand why customers churn, model interpretation techniques were applied:

* Feature importance analysis using Random Forest

* Identification of key churn drivers such as contract type, tenure, monthly charges, and customer support interactions

This step ensures the model is interpretable and actionable for business use.

**11. Business Recommendations**

Based on model results and data insights, the following recommendations were made:

* Customers on monthly contracts have higher churn risk and should be targeted with retention offers

* High customer support interactions indicate dissatisfaction and require proactive engagement

* New customers with high monthly charges should be offered onboarding incentives

**12. Conclusion**

This project successfully demonstrates an end-to-end Machine Learning workflow for customer churn prediction. It combines data preprocessing, feature engineering, model building, evaluation, and business insights. The project aligns with industry practices and is suitable for academic submissions, internships, and interview discussions.
