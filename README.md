# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step1 : 
import pandas as pd.
## Step2 :
Read the csv file.
## Step3 :
Get the value of X and y variables.
## Step4 : 
Create the linear regression model and fit.
## Step5 :
Print the predicted output.

## Program:
```
REGISTER NUMBER: 212224100043
COMPLETED BY: Prathikshaa




import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for corresponding Weight and Volume",predictedCO2)










```
## Output:
<img width="1049" height="493" alt="image" src="https://github.com/user-attachments/assets/bcc739c8-b4a9-4a0a-bdf1-ffa343a56d28" />


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
