# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import the standard libraries.
2.Upload the dataset and check for any null values using .isnull() function.
3.Import LabelEncoder and encode the dataset.
4.Import DecisionTreeClassifier from sklearn and apply the model on the dataset.
5.Predict the values of array.
6.Import metrics from sklearn and calculate the accuracy of the model on the dataset.
7.Predict the values of array.
8.Apply to new unknown values.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: u,srinivas
RegisterNumber:  212221230108

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics   
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
### Data Head:

![1](https://user-images.githubusercontent.com/93427183/171145219-cb39a006-c2ec-4ac2-ad1c-7cb8e54b46f4.png)
### Data Info:

![2](https://user-images.githubusercontent.com/93427183/171145267-40599aab-fb9f-4b72-a498-0799ad1c735d.png)
### Data Isnull:
![3](https://user-images.githubusercontent.com/93427183/171145419-fb2062b3-11c0-4c4b-b808-8975c0c6efef.png)
### Data Left:

![4](https://user-images.githubusercontent.com/93427183/171145526-9f17e297-9221-402e-9291-943dc53238c7.png)
 ### Data Head:
 
![5](https://user-images.githubusercontent.com/93427183/171145683-1b8b82ff-2846-4be5-bde7-51af2591f30c.png)
 ### X.Head:
 ![6](https://user-images.githubusercontent.com/93427183/171145876-5b595b2d-e18a-4bb9-8b6e-c59bb5b51b7c.png)
### Data Fit:
![7](https://user-images.githubusercontent.com/93427183/171145951-262b42be-ed4c-43e2-a2a2-2c0e9574b203.png)
### Accuracy:
![8](https://user-images.githubusercontent.com/93427183/171146062-a3fa9f91-69ec-4508-8ff9-47fb530ebb77.png)

### Predicted Values:
![9](https://user-images.githubusercontent.com/93427183/171146189-3541d8d2-e6f2-4264-8d42-f4a94737841a.png)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
