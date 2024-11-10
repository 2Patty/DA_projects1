Telecommunication Customer Churn Analysis and Prediction
This project aims to build a machine-learning model to predict customer churn for a telecommunications company. Customer churn in this context refers to clients ceasing to use the company's products or services. By identifying churn drivers and predicting churn, this project provides insights to help the company retain valuable customers and increase loyalty, directly contributing to revenue.

Project Overview
Background
In the telecommunications industry, customer retention is crucial, as acquiring new customers is more costly than retaining existing ones. This analysis uses machine learning to help the company understand churn drivers, classify high-risk customers, and identify strategies to reduce attrition.

Objective
Primary Objective: Predict which customers are most likely to churn.
Secondary Objective: Identify the main factors contributing to churn and create strategies to enhance customer retention.
Dataset
The dataset is split into three parts:

Training Data (3000 records) - Contains customer demographics, subscription type, monthly charges, tenure, and churn status.
Validation Data (2000 records) - Extends the training data to improve model performance.
Testing Data (2000 records) - Used for final model testing, estimating real-world model accuracy.
The datasets are stored across an SQL Server database, a GitHub repository, and an Excel file on OneDrive.

Methodology
This project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework:

Business Understanding: Define objectives, such as identifying high-risk customers and key churn drivers.

Data Understanding: Gain insight into the data distribution, missing values, and key attributes related to churn.

Data Preparation:

Missing Value Handling: Impute or remove missing values.
Data Cleaning: Remove duplicates and correct data inconsistencies.
Feature Engineering: Generate features such as customer lifetime value and average monthly spending.
Normalization and Encoding: Normalize numerical features and encode categorical variables.
Modeling:

Train multiple machine learning models, including Logistic Regression, Decision Trees, Random Forest, and Support Vector Machines (SVM).
Perform hyperparameter tuning to optimize model performance.
Evaluation:

Use metrics such as accuracy, precision, and recall to assess model performance.
Explain model predictions with LIME and SHAP to make results interpretable.
Deployment:

Develop an application with pages for data display, prediction, and dashboard visualizations.
Model Performance
The Random Forest model emerged as the best performer. Additional models evaluated include Gradient Boosting, SVC, K-Nearest Neighbors, and Logistic Regression. 

Key Insights
High Monthly Charges: Customers with higher monthly charges show a higher tendency to churn.
Contract Type: Month-to-month contracts are associated with higher churn rates.
Tenure: Shorter tenure is linked to a higher likelihood of churn.
Bundled Services: Customers without bundled services (e.g., internet, TV) are more likely to churn.
Geographic Influence: Location may play a role in churn propensity.
Tools and Technologies
Data Processing: Python (Pandas, Scikit-Learn)
Deployment: Custom application with pages for data, predictions, and dashboards
How to Run
pip install -r requirements.txt
Set up data sources (SQL Server, GitHub, and OneDrive).
Run the Jupyter notebook or the provided scripts to preprocess data, train the models, and evaluate.
License
This project is licensed under the MIT License.

