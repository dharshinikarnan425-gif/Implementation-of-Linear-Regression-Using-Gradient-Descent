# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to predict the profit of a city using the linear regression model with gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

##  Algorithm
1. Read the input values X (independent variable) and y (dependent variable).

2. Assume a linear relationship between X and y using the for p

3. Predict the output values using: pp

4.Display the slope 𝑚 and intercept c, and plot:

Actual data points

Regression line
## Program:
```
/*
Program to implement the linear regression using gradient descent.
Developed by: Dharshini k
RegisterNumber:  25004639
*/
import numpy as np
from sklearn.linear_model import LinearRegression
import matplotlib.pyplot as plt

# Sample data (X = input, y = output)
X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
y = np.array([2, 4, 5, 4, 5])

# Create and train the model
model = LinearRegression()
model.fit(X, y)

# Make predictions
y_pred = model.predict(X)

# Print results
print("Slope (Coefficient):", model.coef_[0])
print("Intercept:", model.intercept_)

# Plot the data and regression line
plt.scatter(X, y, color='blue', label='Actual Data')
plt.plot(X, y_pred, color='red', label='Regression Line')
plt.xlabel("X")
plt.ylabel("y")
plt.legend()
```

## Output:
![linear regression using gradient descent](sam.png)
<img width="1012" height="800" alt="image" src="https://github.com/user-attachments/assets/22c8e455-44db-4972-b9a9-70658e8f8e8f" />


## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
