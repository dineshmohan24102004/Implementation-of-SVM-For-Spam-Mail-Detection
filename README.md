# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program.
   
2.Import the python pandas library as pd.

3.Read the contents of the Spam csv file.

4.Display the first 5 rows of the dataset using head().

5.Assign x as v1 values and y as v2 values.

6.From sklearn library select the feature extraction and import CountVectorizer.

7.CountVectorizer will convert the Text to Numerical Data.

8.From sklearn library import Support Vector Classifier (ie. SVC).

9.Predict the x_test using SVC.

10.Print the accuracy of the SVM Model.

11.Stop the program
   

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Dinesh.M
RegisterNumber:  212222040039



import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["EmailText"].values
y=data["Label"].values
import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["EmailText"].values
y=data["Label"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extractiaon.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
## data.head()
![image](https://github.com/dineshmohan24102004/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119478475/e415e2ff-ce6e-4151-adf3-c6d71ff87e3a)
## data.info()
![image](https://github.com/dineshmohan24102004/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119478475/57e5f1f1-1b2e-4fb1-a8e7-2748e7c80da0)
## data isnull()& sum()
![image](https://github.com/dineshmohan24102004/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119478475/a9e2cfe2-0551-43e3-a03a-4e0385336790)
## Y_prediction()
![image](https://github.com/dineshmohan24102004/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119478475/c8bcb1c8-986d-4f0b-baa3-8b3116b2e4f4)
## Accuracy:
![image](https://github.com/dineshmohan24102004/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119478475/bffbd031-3966-4240-b29a-1465c4087075)









## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
