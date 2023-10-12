# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:

1. Import the required libraries.
2. Upload the csv file and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree inport DecisionTreeRegressor.
5. Import metrics and calculate the Mean squared error.
6. Apply metrics to the dataset, and predict the output.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SWETHA.S
RegisterNumber: 212222230155
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data[["Salary"]]
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test, y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:

data.head():

![Screenshot 2023-10-12 090223](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/368dce81-c0ad-4477-a051-a332a58701fe)

data.info():

![Screenshot 2023-10-12 090228](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/aafe33b1-80ad-4db6-9153-87e15635da7f)

data.isnull().sum():

![Screenshot 2023-10-12 090651](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/b85967ac-f73a-4791-acf8-4b36207cabca)

data.head() for salary:

![Screenshot 2023-10-12 090934](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/d5a2007a-0ea4-49fe-907b-89ceb313ad46)

MSE:

![Screenshot 2023-10-12 091726](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/c538b1ba-6ce8-46a4-9167-87c1c9b639a0)

r2 value:

![Screenshot 2023-10-12 091859](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/32f4ed9e-2725-4688-b3f1-718923d7b28e)

Data prediction:

![Screenshot 2023-10-12 092446](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119525603/930f0531-781b-47b4-8154-8e955f66a927)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
