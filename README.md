# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Get the independent variable X and dependent variable Y.

### Step2
<br>Calculate the mean of the X -values and the mean of the Y -values.

### Step3
<br>Find the slope m of the line of best fit using the formula.

### Step4
<br>Compute the y -intercept of the line by using the formula:

### Step5
<br>Use the slope m and the y -intercept to form the equation of the line.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv(r"C:\Users\acer\Downloads\car (1).csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:
<img width="786" height="365" alt="image" src="https://github.com/user-attachments/assets/817e3d8a-4096-4b38-87ac-39aa86126fa6" />

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
