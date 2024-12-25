# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by:MADHAN C
RegisterNumber:24004329
import chardet
file = "/content/spam.csv"
with open(file, 'rb') as rawdata:
    result = chardet.detect(rawdata.read(100000))
result
import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding='Windows-1252')
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extraction.text import CountVectorizer
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
![SVM For Spam Mail Detection](sam.png)
![Screenshot 2024-12-25 215455](https://github.com/user-attachments/assets/00459c7b-3b32-4fc7-b007-17f71526a7a0)
![Screenshot 2024-12-25 215510](https://github.com/user-attachments/assets/3b340805-6cd2-4626-b354-16477f52f6d9)
![Screenshot 2024-12-25 215522](https://github.com/user-attachments/assets/766664b3-ba14-48de-b614-306d5d0345e6)
![Screenshot 2024-12-25 215529](https://github.com/user-attachments/assets/6065ffe5-edd4-42df-ae61-ad212ecf4704)
![Screenshot 2024-12-25 215544](https://github.com/user-attachments/assets/9ad992f0-c3dc-4413-aadd-a80843b86c91)
![Screenshot 2024-12-25 215548](https://github.com/user-attachments/assets/1ae5ea3d-65e9-4ec4-a799-c764eeff2989)
![Screenshot 2024-12-25 215555](https://github.com/user-attachments/assets/66b403b6-41dd-4fa8-8678-f56f5347db44)
![Screenshot 2024-12-25 215603](https://github.com/user-attachments/assets/21d04595-aa5f-47fb-8554-b932a4abeb34)
![Screenshot 2024-12-25 215611](https://github.com/user-attachments/assets/1c9f9d8f-8e8c-415b-8194-42b15846dbc8)
![Screenshot 2024-12-25 215618](https://github.com/user-attachments/assets/f3dd0974-8b1d-45c7-a1d1-3582a21166a2)
## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
