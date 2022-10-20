---
title: "The page for pandas knowledge"
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

