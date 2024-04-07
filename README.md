# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: MIDHUN S
RegisterNumber:  212223240087

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()    #no departments and no left
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
#### data.head()
![exp 8 1](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/885d6139-399a-4c19-a3a0-db05ea5f3893)

#### data.info()
![exp 8 2](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/80cf87e6-649a-4ed3-abf1-b626c8e39455)


#### isnull() and sum()
![exp 8 3](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/5e2e4149-0a0a-4a6a-8dd9-cf007fa89b10)


#### data value counts()
![exp 8 4](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/7bda7406-970c-4569-bada-53f45bdb6cef)


#### data.head() for salary
![exp 8 5](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/b38d765b-244a-4814-af3c-29e2c25908a8)


#### x.head()
![exp 8 6](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/ad7ad011-7a8f-40de-8eb2-d6dabaa54981)


#### accuracy value
![exp 8 7](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/f330326b-c3dd-4313-99de-2f616067fa06)

#### data prediction
![exp 8 8](https://github.com/23003250/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331462/0a7b6663-9df1-4112-b407-8596359ed10f)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
