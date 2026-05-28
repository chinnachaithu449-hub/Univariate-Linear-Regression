# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output
<img width="744" height="603" alt="WhatsApp Image 2026-05-28 at 6 53 34 PM" src="https://github.com/user-attachments/assets/92362ed2-969c-4852-8465-d5eabebb014e" />
<img width="702" height="517" alt="WhatsApp Image 2026-05-28 at 6 53 49 PM" src="https://github.com/user-attachments/assets/d12432c3-6278-40b4-b67f-804e6ad3c69a" />




## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
