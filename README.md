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
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Renuga.S
Register number: 212222230118
import numpy as np
import matplotlib.pyplot as py
x=inp.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num,denom=0,0
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-(m*x_mean)
print(m,b)
y_pred=(m*x)+b
print(y_pred)
py.scatter(x,y,color='purple')
py.plot(x,y_pred,color="red")
py.show()
```




## Output
![mathplot](https://github.com/RENUGASARAVANAN/Univariate-Linear-Regression/assets/119292258/0dd3b397-5a69-4516-8be8-4a511f35d928)



## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
