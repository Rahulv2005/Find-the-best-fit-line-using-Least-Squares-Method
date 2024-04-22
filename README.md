# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Rahul V
RegisterNumber: 212223240132
```


import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='blue')
plt.plot(X,Y_pred,color='yellow') 
plt.show()
```

## Output:
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/e367ae78-cc0c-4e9b-b5f6-46cea2f37b75)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/d25a849c-834a-4bec-925b-f64546590785)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/d1d25620-b1a6-4a5e-bd5c-f5378823d8aa)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/f25e2e4a-5932-471a-ac24-b2fba517da31)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/efce4e13-9ac0-444e-8b80-a2b59ceb0a2b)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/fbac68ef-2f1a-43c4-87d2-f6857f878ff0)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/20168739-d83c-42c4-be0c-28eea8fd5320)
![image](https://github.com/Rahulv2005/Find-the-best-fit-line-using-Least-Squares-Method/assets/152600335/271a612d-0a20-4fb6-bf4b-5a078e02954a)




## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
