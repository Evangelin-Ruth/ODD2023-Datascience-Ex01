## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE
```
import pandas as pd

df=pd.read_csv("SAMPLEDS.csv")

df

df.head

df.tail

df.info()

df.describe()

df.shape

df.isnull().sum()

df.dropna(how='any').shape

x=df.dropna(how='any')

x

df.dropna(how='all').shape

df

tot=df.dropna(subset=['TOTAL'],how='any')

tot

tot=df.dropna(subset=['M1','M2','M3','M4'],how='any')


tot

df.fillna(0)

df

df.fillna(method='ffill')

df.fillna(method='bfill')

df.interpolate()

mn=df.TOTAL.mean()

mn

df.TOTAL.fillna(mn,inplace=True)

df

l=df.M1.interpolate()

l

df.M1.fillna(l,inplace=True)

df

mn=df.TOTAL.median()
mn

mn=df.TOTAL.mode()
mn

df.isnull()

df

df.duplicated()

df.drop_duplicates(inplace=True)

df

df['cd']=pd.to_datetime(df['DOB'])

df

for x in df.index:
  if df.loc[x,"AVG"]>100:
    df.drop(x,inplace=True)

df
```

# OUTPUT
![ds op2](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/b76e3234-a4bc-4a61-8db9-837e859ed050)
![ds op4](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/221bede1-369a-45ba-a732-0020ddc12c78)
![ds op5](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/fa8cf364-e20a-4ae6-b5b8-9e566d935344)
![ds op6](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/f0e5bc94-0db3-4f03-bb84-e0700e288ed0)
![ds op7](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/a09717b9-f8e3-4817-ade4-65b7e8f1ba3e)
![ds op8](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/43dacd53-8db4-4342-b92c-ae991e4499b4)
![ds op10](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/5d0f72f8-d4d7-46f8-bb08-8740fb4ba1ce)
![ds op15](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/3073a1cf-e8d6-4992-a5a9-2f54b66d6187)
![ds op17](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/d2dab6cb-a109-48d9-8088-b60e050c5d33)
![ds op18](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/08ac3365-6415-4642-85e8-818a2c418440)
![ds op19](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/42beaef8-9f2e-4b00-854e-8cc982f643d4)
![ds op20](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/3f93111f-42a0-45e3-ac2c-2baf898a22bd)
![ds op21](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/77c1a2d7-48cb-4709-9ade-ae99aaaba27b)
![ds op22](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/c9e9f0ed-cb91-4082-92a7-7e02baf29a5e)
![ds op23](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/597f662a-7291-4ca6-9422-ccfc7db3be67)
![ds op24](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/4b46a869-c74e-4872-bcb1-9ea1e60f22e5)
![ds op25](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/17b4174d-844c-450b-91b8-d9dd275fb4e6)
![ds op26](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/c1271cd8-5862-4a6e-8cba-07fd5468e495)
![ds op28](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/90fd641d-ce13-49fb-9637-b362fb09a04c)

















