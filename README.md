# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Select any online compiler.
### Step2
Type the required coding.
### Step3
Import pandas.
### Step4
Take a screenshot of the output and copy the program and the output in your git repository.
### Step5
Push the output images and program in the git repository.
## Program:
```
'''
Developed by: SUDHARSAN RAM M
Reference number: 212222110048
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
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
![Screenshot 2023-11-18 084844](https://github.com/Sudharsanram/Multivariate-Linear-Regression/assets/119393980/e0a42e07-7fb2-4e89-93c6-0a0f1729ffa9)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
