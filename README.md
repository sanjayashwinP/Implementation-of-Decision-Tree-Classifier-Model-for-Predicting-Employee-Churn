# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.

2.Read the data set.

3.Apply label encoder to the non-numerical column inoreder to convert into numerical values.

4.Determine training and test data set.

5.Apply decision tree Classifier and get the values of accuracy and data prediction.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SANJAY ASHWIN P
RegisterNumber:  212223040181

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

![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/ed79af91-9c82-4f49-8cdb-5f7cfc1a5d43)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/61d97465-5faa-42f9-81f3-bf7baaba5ebf)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/10527a8a-5a88-4129-addc-836a038b8cf0)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/fe4b54bc-fe64-4029-b0be-ba9761c76873)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/98219ca6-7f80-422c-8ebb-0e4c3e49b661)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/16db89bd-58bd-4a84-80c1-50f1bfb7cb6a)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/7098c8c4-323a-4050-a3cf-01a8ff84bc24)


![image](https://github.com/sanjayashwinP/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/147473265/99c7efee-6b78-47aa-8cc1-92d88c670697)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
