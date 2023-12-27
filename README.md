# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

Import the pandas and scikit-learn libraries

### Step2
Read the data from the csv file.
### Step3
Split the data into features (X) and target(y)

### Step4
Create and fit the linear linear regression model.
### Step5
Print the coefficients and intercepts of the linear regression model.

### Step6
Make a prediction.

## Program:
```py
#Implementation of Multivariate Linear Regression
#Developed by: HARISHKUMAR R
#Register Number: 212223230073

import pandas as pd
from sklearn import linear_model

data = pd.read_csv("cars (1).csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("Intercept",regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print("predicted CO2 for te corresponding weight and volume",predictCO2)






```
## Output:

![](./OUT.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.