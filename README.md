# Customer Churn Prediction in the Telecommunications Industry
<img width="960" alt="coverimage" src="https://github.com/EstonKamau/Phase3-Project/assets/124604037/d8572360-b156-4f26-9174-52c6ca67b794">


## Project Overview
The goal of this project is to build a classifier that can predict whether a customer of SyriaTel, a telecommunications company, is likely to churn or not. Churn refers to customers who stop doing business with a company, and predicting churn is crucial for businesses to retain customers and reduce financial losses.

By analyzing a dataset obtained from Kaggle, we aim to identify patterns and factors that contribute to customer churn in the telecommunications industry. Through machine learning techniques and predictive modeling, we will develop a classification model that can accurately predict churn.

This project not only focuses on building an accurate churn prediction model but also aims to provide actionable recommendations based on the insights gained from the analysis.


## Business Understanding
The telecommunications industry is highly competitive, and customer retention is crucial for the success and profitability of telecom companies. Customer churn, or when customers switch to competitors or discontinue their services, can result in significant financial losses. It is important for telecom companies to identify and understand the factors that contribute to customer churn in order to implement effective retention strategies.

SyriaTel, as a telecommunications company, is interested in reducing the financial impact of customer churn. By predicting customer churn in advance, SyriaTel can proactively intervene and implement targeted retention efforts to retain customers who are at high risk of leaving. This project aims to develop a classifier using machine learning techniques to predict whether a customer will "soon" stop doing business with SyriaTel.


## Objectives
* Understanding the relationship between the customer churn and other variables
* To understand what variables have a huge influence on customer decision to churn
* Develop a machine learning model that can classify customers as either likely to churn or likely to continue using SyriaTel's services


## Usage
* git clone https://github.com/EstonKamau/Phase3-Project.git
* install the necessary libraries
* Run the project
Make sure you have Python (version X.X.X) installed on your system.


## Data Understanding
The dataset had 3333 rows and 21 columns.
There were no missing values.
There were no duplicated values.

The following are the categorical variables: 
***state, phone number, international plan, voice mail plan*** 

The following are the numerical variables:
***account length, area code, number vmail messages, total day minutes, total day calls, total day charge, total eve minutes, total eve calls, total eve charge, total night minutes, total night calls, total night charge, total intl minutes, total intl calls, total intl charge, customer service calls***


## Data Preparation
* To make the analysis a lot clearer, I summed up the:
  * 'total day minutes', 'total eve minutes’ , 'total night minutes’  and created a new variable: ***total minutes***
  * 'total day charge', 'total eve charge’ , 'total night charge’  and created a new  variable: ***total charge***
  * 'total day call', 'total eve call’ , 'total night call’  and created a new variable: ***total call***
* Area code variable was converted to a categorical variable since it only had unique variables
* Used SMOTE to address class imbalance in the dataset.


## Modelling and Evaluation
Three models: Decision Tree Model, Random Forest Model and Random Forest with tuned Hyperparameters Model, were trained and evaluated using appropriate evaluation metrics.
Feature importance as well as cross-validation was performed for each model.


## Results
Random Forest model with tuned hyperparameters proves to be the best as it has the best metric scores between all the 3 models. This means it correctly classifies the highest amount of customer churn cases.
It provides a good balance between accuracy and recall, indicating its ability to correctly identify customers who are likely to churn. 

Total charge tends to appear as the most important feature in all the 3 models. Perhaps, SyriaTel should consider on reducing their charges as a way of reducing customer churn

<img width="335" alt="image" src="https://github.com/EstonKamau/Phase3-Project/assets/124604037/3e667f21-abe5-4b96-9c6f-372f35470c0c">


## Future Work
Conduct a comprehensive business impact analysis to assess the financial implications of implementing the model's predictions. 

## Contibutors
Eston Kamau


## Contact
Email: muraguriestonk@gmail.com

