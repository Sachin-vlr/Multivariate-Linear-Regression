# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas

### Step2
Import linear_model

### Step3
Read the csv file

### Step4
Enter the parameters to implement

### Step5
Run the program and predict the output

## Program:
```python
#DEVELOPED BY : SACHIN.C
#REG NO. : 22001187
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars.csv")
x=data[["Weight","Volume"]]
y=data["CO2"]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("coefficients: ",regr.coef_)
print("intercept:",regr.intercept_)
predictco2=regr.predict([[3300,1300]])
print("prediction co2 for the corresponding weight and volume",predictco2)
```







## Output:
![output](/MULTI.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.