# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:
Import libraries (numpy, pandas, sklearn).
### Step 2: 
Load data and separate features (X) and target (y).
### Step 3: 
Split data into training and testing sets.
### Step 4: 
Train LinearRegression model on training data.
### Step 5: 
Predict outputs and evaluate the model.

## Program:
```
Program for Multivariate linear regression using the least squares method.
Developed by: HITHESHHWARAN AR
RegisterNumber: 212224040118
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/car (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
<img width="1409" height="485" alt="image" src="https://github.com/user-attachments/assets/ea2dde5c-110e-4f88-9a57-ac9f624a16d6" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
