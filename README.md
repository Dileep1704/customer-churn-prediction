Customer Churn Prediction

Project Overview

This project focuses on predicting customer churn using machine learning techniques. Customer churn refers to customers who stop using a company’s services. Predicting churn helps companies identify high-risk customers and improve customer retention strategies.

In this project, telecom customer data is analyzed to understand factors influencing churn and to build predictive models.

Dataset

The dataset used in this project is the Telco Customer Churn dataset. It contains information about customers such as:

tenure – number of months the customer stayed with the company  
Contract – type of contract (month-to-month, one year, two year)  
MonthlyCharges – monthly subscription cost  
TotalCharges – total amount paid by the customer  
PaymentMethod – payment method used  
Churn – indicates whether the customer left the service  

Project Workflow

The project follows a typical data science workflow.

Data Cleaning  
Handling missing values and correcting data types.

Exploratory Data Analysis  
Understanding patterns and relationships between features and churn.

Feature Engineering  
Creating additional features such as contract risk and tenure risk.

Handling Class Imbalance  
Using SMOTE to balance the churn and non-churn classes.

Model Training  
Training multiple machine learning models.

Model Evaluation  
Comparing model performance using accuracy and ROC-AUC.

Models Used

Logistic Regression  
Random Forest  
XGBoost

Results

Among the models tested, XGBoost produced the best performance for churn prediction. The models were evaluated using accuracy, confusion matrix, and ROC-AUC score.

Key Insights

Customers with month-to-month contracts are more likely to churn.  
Customers with shorter tenure tend to leave the service earlier.  
Higher monthly charges increase churn probability.  
Customers with more services are less likely to churn.

Project Structure

customer-churn-prediction

data  
Telco-Customer-Churn.csv  

notebooks  
churn_analysis.ipynb  

images  
churn_distribution.png  
feature_importance.png  

models  
churn_model.pkl  
scaler.pkl  

requirements.txt  
README.md

How to Run the Project

Install the required libraries:

pip install -r requirements.txt

Open the notebook in Jupyter:

notebooks/churn_analysis.ipynb

Run the notebook cells to reproduce the analysis and train the models.

Future Improvements

Deploy the model as a web application for real-time churn prediction.  
Experiment with additional machine learning algorithms.  
Perform hyperparameter tuning to improve performance.