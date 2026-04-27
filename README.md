# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to predict the profit of a city using the linear regression model with gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import required libraries and initialize input (X) and output (Y) data.


2. Create and train the Linear Regression model using model.fit(X, Y).


3. Find slope and intercept of the regression line.


4. Get user input and predict the marks using the trained model.


5. Plot the actual data and regression line using a graph.
## Program:
```
/*
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
data = pd.read_csv(r"C:\Users\Yazhini\Downloads\Startup (1).csv")

# Select one feature (R&D Spend) and target (Profit)
X = data['R&D Spend'].values
y = data['Profit'].values

# Normalize (important for gradient descent)
X = (X - X.mean()) / X.std()

# Initialize parameters
m = 0
b = 0

learning_rate = 0.01
epochs = 1000
n = len(X)

# Gradient Descent
for i in range(epochs):
    y_pred = m * X + b
    
    # Gradients
    dm = (-2/n) * np.sum(X * (y - y_pred))
    db = (-2/n) * np.sum(y - y_pred)
    
    # Update
    m = m - learning_rate * dm
    b = b - learning_rate * db

print("Slope (m):", m)
print("Intercept (b):", b)
y_pred = m * X + b

# Predictions for plottin

# Plot
plt.scatter(X, y)
plt.plot(X, y_pred)

plt.xlabel("R&D Spend (Normalized)")
plt.ylabel("Profit")
plt.title("Gradient Descent on 50_Startups Dataset")

plt.show()
Developed by: 
RegisterNumber:  
*/
```

## Output:
![linear regression using gradient descent](sam.png)

<img width="840" height="610" alt="image" src="https://github.com/user-attachments/assets/97e9eff4-44b9-47fe-b6b9-7703d19bea9e" />

Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
