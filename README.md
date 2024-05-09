# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
### Step2
Read the csv file.
### Step3
Get the value of X and y variables
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.


## Program:
```
#Developed by:KANNAN.S
#Rgister number: 212223230098

import pandas as pd
from sklearn import linear_model
data=pd.read_csv('car (2).csv')
x=data[['Weight','Volume']]
y=data['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("coefficient:",regression.coef_)
print("Intercept:",regression.intercept_)
predictCO2=regression.predict([[3300,1300]])
print("co2 required is",predictCO2)

```

## Output:
![image](https://github.com/Kannan-S-coder/Multivariate-Linear-Regression/assets/147120710/3e6af3cb-16d9-44ac-a63d-fb6975131894)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
