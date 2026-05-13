# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Load the employee salary dataset.
2. Train the Decision Tree Regressor model using input features.
3. Predict the salary for new employee data.
4. Compare predicted salary with actual salary to measure accuracy.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Ritika S
RegisterNumber:  212225220086
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeRegressor, plot_tree
data = pd.read_csv("Salary (1).csv")
X = data.drop("Salary", axis=1)
y = data["Salary"]
X = pd.get_dummies(X, drop_first=True)
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42)
model = DecisionTreeRegressor(random_state=42)
model.fit(X_train, y_train)
plt.figure(figsize=(25,12))
plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)
plt.title("Decision Tree Regressor")
plt.show()
*/
```
## Output:
![Decision Tree Regressor Model for Predicting the Salary of the Employee](sam.png)
<img width="987" height="832" alt="Screenshot 2026-05-13 093550" src="https://github.com/user-attachments/assets/82b52296-6763-4495-92ff-d37999c6c281" />
## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
