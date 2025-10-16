# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Load the dataset using pandas.

### Step2
Select input features (Weight, Volume) and target variable (CO2).

### Step3
Create and train the Linear Regression model using the selected data.

### Step4
Display the model’s coefficients and intercept.

### Step5
Predict CO2 emission for given input values (3300, 1300).

## Program:
```
import pandas as pd

from sklearn import linear_model

df=pd.read_csv("C:\\Users\\admin\\Downloads\\car (1).csv")

df

x=df[['Weight', 'Volume']]

y=df['CO2']

regr=linear_model.LinearRegression()

regr.fit(x,y)

print('Coefficients: ',regr.coef_)

print('Intercept:',regr.intercept_)

predictedCO2=regr.predict([[3300,1300]])

print("Predicted:",predictedCO2)

```
## Output:
<img width="1422" height="635" alt="image" src="https://github.com/user-attachments/assets/c229da19-9323-419f-b66d-3724a32b1188" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
