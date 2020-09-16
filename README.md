# Predicting-Credit-Card-Approvals

|| Introduction

In this project, I tried to build a model that can help banks decide whether a client can be approved for a credit cards


|| Languages & Tools

Python & Jupyter Notebook


|| Methodologies

First, I inspected the data, which contained Gender, Age, Debt, Married, BankCustomer, EducationLevel, Ethnicity, YearsEmployed, PriorDefault, Employed, CreditScore, DriversLicense, Citizen, ZipCode, Income and finally the ApprovalStatus
I understood that some of the factors mentioned above may be correlated to the final approval, some of them may not have correlation with it.
Moreover, the data's types have both numeric and categorical, meaning I need different methods to manipulate and preprocessing them.

Then, I replaced the missing with np.nan. I imputed the numeric value using mean imputation. Also, I imputed the categorical value with the most frequent value of the column

Thrid, I pre-processed the data by the following steps:

 (1)Converting the non-numeric data into numeric - LabelEncoder (from sklearn import preprocessing)
 
 (2)Spliting the data into train and test sets - training data:testing data = 2:1 (from sklearn.model_selection import train_test_split)
 
 (3)Scaling the feature values to a uniform range - MinMaxScaler (from sklearn.preprocessing import MinMaxScaler)

Last but not least, I fitted a logistic regression model and inspected it's performance:

 (1)Fitting logistic regression model - assumed features are correlated with each other,on, used generalized linear models (Logistic Regression model) - (from sklearn.linear_model import LogisticRegression)
 
 (2)Evaluating performance - confusion matrix (from sklearn.metrics import confusion_matrix)
 
 (3)Making the model perform better - Grid Search (from sklearn.model_selection import GridSearchCV)
 
 
|| Project Resources & Data

DataCamp
