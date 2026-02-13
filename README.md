📊 Telecom Churn Prediction Project
📌 Project Overview

This project analyzes customer churn for a telecom company and builds a predictive model to identify customers at risk of leaving the service.

The objective is to:

Perform data quality analysis

Conduct Exploratory Data Analysis (EDA)

Identify key business insights

Build predictive models for churn

Explain the main churn drivers

Provide operational recommendations

📂 Dataset Description

The dataset contains 1200 customers with 11 variables, including:

customer_id – unique identifier

age – customer age

tenure_months – months since subscription

monthly_charge – monthly payment amount

contract_type – month-to-month / one year / two year

internet_service – DSL / Fiber / other

tech_support – Yes / No

streaming_tv – Yes / No

payment_method – payment type

num_support_tickets – number of customer service tickets

churn – target variable (Yes / No)

🧹 Data Preparation

The following preprocessing steps were performed:

Removed customer_id (non-informative identifier)

Handled missing values in internet_service

Converted churn into binary format (1 = churn, 0 = no churn)

Applied one-hot encoding to categorical variables

Split dataset into training (80%) and test (20%) sets using stratification

📊 Exploratory Data Analysis (EDA)

EDA revealed:

Strong Drivers of Churn:

Contract Type (month-to-month customers churn more)

Tech Support (customers without support churn more)

Moderate Drivers:

Number of support tickets

Internet service type

Weak Drivers:

Age

Tenure

Monthly charge

Streaming TV

Payment method

🤖 Predictive Modeling

Two classification models were trained:

1️⃣ Logistic Regression (Baseline Model)

Accuracy ≈ 66%

Moderate recall for churn detection

2️⃣ Random Forest Classifier

Accuracy ≈ 66%

ROC-AUC ≈ 0.72

Better ability to capture nonlinear patterns

The dataset shows moderate predictability, which is realistic for churn problems.

🔍 Key Findings

The most influential variables are:

Contract type

Tech support

Number of support tickets

Tenure and monthly charge (non-linear impact)

Churn is primarily driven by service experience and contract flexibility, not demographics.

💡 Business Recommendations

Based on the analysis:

Encourage long-term contracts with incentives

Improve and promote technical support services

Monitor customers with high support ticket activity

Use the predictive model to target high-risk customers

Focus on service quality rather than aggressive price discounts

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Scikit-learn

📈 Future Improvements

Hyperparameter tuning

Testing Gradient Boosting models

Feature engineering (interaction terms)

Incorporating customer behavior data

🎯 Conclusion

This project demonstrates how data analysis and machine learning can:

Identify churn drivers

Predict customer behavior

Support data-driven strategic decisions

While the model achieves moderate predictive performance, it provides actionable insights that can reduce churn and improve customer retention.
