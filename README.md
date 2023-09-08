# Waze
Data analysis of Waze project (part of Google Advanced Data Analytics Certification)
This project is completed as a part of the Google Advanced Data Analytics Capstone Project.
It utilizes data analytics concepts and techniques covered in the professional certification course.

## Overview
Waze is a fictitious company created for educational purposes only and any reference is coincidental.
Waze is a navigational app which guides users from one location to another. It has seen a decline in its usage
and has requested an analysis of their user data to predict user churn.

## Objectives
- Build a model to predict user churn
- Provide insights into the data
- Propose business solutions to prevent user churn
- determine factors affecting user churn
- Conduct Exploratory data analysis

## Analysis
A PACE strategy document was formulated to initiate the process and workflow.
An initial exploratory data analysis was conducted and the dataset was cleaned and structured for modelling.
The dataset had 18% of users who churned. They drove 200 kilometers more and for 2.5 hours more when compared with retained users
in the last month. No. of driving days negatively affected the user churn. Users who used the app more were less likely to churn.
Users who used an iPhone had more No. of drives.
A machine learning model was built to predict if a user will churn using different methods such as Random Forest Classification,
Logistic Regression, Extreme Gradient Boosting and Decision Tree Classifier.

## Results
The results of the analysis were as follows:
- Recall score was a key score to the models
- Activity days was the most important feature which was negatively correlated to churn.
- Distance driven per day was one of the least important variables.
- Engineered features had the highest factor in the model's prediction
- XGBoost model performed better than the random forest model.

## Solutions
Proposed solutions are as follows :
- Additional data is required to build a robust and reliable model
- Feedback and surveys will prove to be effective in providing an accurate prediction
- Beta testing of the model before deployment is recommended to gain better insights
- Improving user experience to increase the usage of the app will impact the retention positively.

The results of the models are shown in the jupyter notebook, a brief overview of the scores of each model is given below :

|  model	  | precision	| recall	  |    F1     | accuracy |
| --------- | --------- | --------- | --------- | -------- |
|  RF cv	  | 0.457163	| 0.126782	| 0.198445	| 0.818510 |
| XGB cv	  | 0.442586	| 0.173468	| 0.248972	| 0.814780 |
|  RF val	  | 0.445255	| 0.120316	| 0.189441	| 0.817483 |
| XGB val	  | 0.430769	| 0.165680	| 0.239316	| 0.813287 |
| XGB test  | 0.388889  |	0.165680  |	0.232365  |	0.805944 |

**NOTE : Visualizations and charts can be found in the jupyter notebooks and executive summaries of each phase in the PACE strategy lifecycle.**

## Libraries Used
- numpy
- pandas
- sklearn
- xgboost
- matplotlib
- seaborn
