# Customer Churn Prediction

## 📌 Project Overview
This project aims to predict whether a customer will discontinue a subscription-based service using machine learning models. By analyzing historical customer data, including demographic details, subscription duration, and usage patterns, we can identify factors contributing to churn and build a predictive model to assist businesses in retaining customers.

## 📊 Dataset Description
The dataset used for this project contains customer information with the following columns:

| Column Name       | Description |
|------------------|-------------|
| RowNumber       | Row index (removed during processing) |
| CustomerId      | Unique customer identifier (removed) |
| Surname        | Customer surname (removed) |
| CreditScore    | Customer's credit score |
| Geography      | Customer's country (encoded) |
| Gender         | Customer's gender (encoded) |
| Age            | Customer's age |
| Tenure         | Number of years as a customer |
| Balance        | Customer's account balance |
| NumOfProducts  | Number of products the customer has |
| HasCrCard      | Whether the customer has a credit card (1 = Yes, 0 = No) |
| IsActiveMember | Whether the customer is an active member (1 = Yes, 0 = No) |
| EstimatedSalary | Estimated salary of the customer |
| Exited         | Target variable (1 = Churned, 0 = Not Churned) |

## ⚙️ Installation
Ensure you have Python installed. Install the required libraries using the following command:

bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn


## 🚀 Usage
### 1️⃣ Load the Dataset
Ensure the dataset (Churn_Modelling.csv) is available in the working directory.

### 2️⃣ Run the Model Training Script
Execute the script to train and evaluate the machine learning models:

python
python churn_prediction.py


### 3️⃣ Model Training and Evaluation
The script performs the following steps:
- Loads and cleans the dataset
- Handles missing values using median and most frequent imputation
- Encodes categorical features using one-hot encoding
- Splits the data into training and testing sets
- Scales numerical features using StandardScaler
- Trains and evaluates three models:
  - *Logistic Regression*
  - *Random Forest Classifier*
  - *XGBoost Classifier*
- Displays accuracy and classification reports
- Visualizes feature importance using XGBoost

## 📈 Expected Output
- Model accuracy scores for different classifiers
- A classification report with precision, recall, and F1-score
- A feature importance graph showing key factors influencing churn

## 🔍 Insights & Business Value
- Helps businesses identify at-risk customers and take proactive retention measures
- Provides insights into key factors that drive customer churn
- Supports customer relationship management strategies

## 🏆 Future Improvements
- Implement hyperparameter tuning for better model performance
- Try other advanced models like Neural Networks or Gradient Boosting variations
- Integrate real-time customer data for live churn prediction



