---
title: "Python-Pandas"
date: 2022-10-20
---

```
import os

# get current working directory
cwd = os.getcwd()

# get files in directory
files = os.listdir(cwd) 

print(files)
```


```
# read the csv file from $file_path and the content don't have a header.
import os

cwd = os.getcwd()
print(f'Current Working Directory: {cwd}')
file_path = os.path.join(cwd,'Mall_Customers.csv')
print(f'Path of Data File: {file_path} \n')

df = pd.read_csv( file_path, header=None)
df.head()
```

```
import pandas as pd
df = pd.DataFrame(breast_cancer.data, 
                  columns = breast_cancer.feature_names)
df['diagnosis'] = breast_cancer.target
df
```

```
from sklearn.model_selection import train_test_split
X = df.iloc[:,:-1]      
y = df.iloc[:,-1]
#---perform a split---
random_state = 12
X_train, X_test, y_train, y_test = train_test_split(X, y,test_size = 0.3,
                     shuffle = True,random_state=random_state)
```
