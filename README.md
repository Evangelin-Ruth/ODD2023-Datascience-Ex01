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

![ds op27](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/b116f2e8-e224-40a6-acee-ccf1bf46ca04)


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

![ds op1](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/4be55de2-dd02-41aa-b781-cbf12f75702b)
![ds op2](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/b76e3234-a4bc-4a61-8db9-837e859ed050)
![ds op3](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/2a0e8a19-f130-4ed6-918b-953f5bf99e7f)
![ds op4](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/58e0269d-02f1-4e7c-b756-1a306fadcac5)
![ds op5](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/f22905a2-33d5-4330-a91e-5cd117febaa1)

![ds op6](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/c6a48d4e-5437-49ce-a260-69a08e39d046)


![ds op7](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/8ca1967c-4e6c-45d5-9752-66b0670c7cd6)


![ds op8](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/03f47969-5136-4779-adbd-f90c3035292c)


![ds op9](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/574f15fc-ed26-441f-806f-a0c05d28d767)
![ds op10](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/2450437e-d4dd-428b-be99-9abc4726a032)
![ds op11](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/6aabfd8b-0be3-414d-b54b-939681613a32)
![ds op12](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/009c9cf6-56c0-49d5-9638-0452aed5b66c)
![ds op13](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/12efa239-7952-4271-881b-a74e06ce09e7)
![ds op14](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/d698ad15-a6e6-4184-88df-66859a51f8f2)
![ds op15](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/e98a52ae-40ec-438a-b202-c05a4a0aaf1e)
![ds op16](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/25ff00c4-7e65-4562-a4cd-f08f4aabe49e)
![ds op17](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/a8e68cad-9730-46fe-a820-e7b5d3c95d05)
![ds op18](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/fcc27fda-3efc-482b-ac9a-196f11c3e192)
![ds op19](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/faff5e2c-bf6a-44f4-b9ff-5dddf1f0727e)
![ds op20](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/dc5011d3-ea63-43f0-8523-b9bac72659ab)


![ds op21](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/58e19b60-0d9e-4196-a899-aa8f3c5ce47a)


![ds op22](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/07e43672-c445-400a-80a4-5e4e34c2ff73)
![ds op23](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/6865c9a7-cb4a-4159-af0d-36ef2d9e10e1)
![ds op24](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/667b2bb7-5577-4841-a5e9-1af3fcdde46f)
![ds op25](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/6e7f03fd-6cd5-4a95-9ff6-6991a8cc1262)
![ds op26](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/d405d740-1bd0-4721-bffa-6ab195ca3fff)
![ds op27](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/51804d39-7d8b-4774-848c-a3c27bf81a33)
![ds op28](https://github.com/Evangelin-Ruth/ODD2023-Datascience-Ex01/assets/94219798/eafef4a4-6acd-4263-9766-117c713265d4)
















