# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd

### Step2
import pandas as pd.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm.

###Step6
Print the predicted output.

## Program:
```
##Developed by: Meiyarasi.V
##REGISTER NUMBER: 212221230058

import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars.csv")

X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)

print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:
![image](https://user-images.githubusercontent.com/121418418/214926378-8aade468-b7c8-4abc-b263-d1782ff3d997.png)


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
