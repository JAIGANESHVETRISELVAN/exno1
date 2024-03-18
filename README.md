# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
 import pandas as pd
 df=pd.read_csv("/content/Data_set .csv")
 df
 df.head(10)
 df.info()
 df.isnull()
 df.isnull().sum()
 df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
 df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
 df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
 df.head()
 df['rating']=df['rating'].fillna(df['rating'].mean())
 df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean
 df.head()
 df['watchers']=df['watchers'].fillna(df['watchers'].median())
 df.head()
 df.info()
 df.isnull().sum()
 ![Screenshot 2024-03-18 082715](https://githu![Screenshot 2024-03-18 082756](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/cc1c0b3a-d125-4fd0-b310-64c6a2bb89e2)
b.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/4994a8e6-b39a-4b10-882c-cdf080ff86d9)
![Screenshot 2024-03-18 082741](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/607c8a40-38e1-4c96-8dc3-3821b39d6416)
![Screenshot 2024-03-18 082814](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/f2c445ba-15ef-4673-960c-f593960ca016)
![Screenshot 2024-03-18 082829](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/b498b1a3-ffe2-4573-87ea-67190202ca96)
![Screenshot 2024-03-18 082851](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/d12d2252-95f5-4901-a8ab-52b4fd0f1eaf)
![Screenshot 2024-03-18 082905](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/180401aa-d499-4d5a-8deb-9c71a2176d2b)
![Screenshot 2024-03-18 082916](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/b18a0c08-f09b-4a6d-9801-27523b852e35)
![Screenshot 2024-03-18 082942](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/a003ca45-c618-41f5-9cc9-7557212031be)
![Screenshot 2024-03-18 082958](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/d4b8e7de-03d4-4e65-a663-bab2f29a571f)
![Screenshot 2024-03-18 083011](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/662fce93-1c95-4898-a0cc-678e97bd216a)

![Screenshot 2024-03-18 083023](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/6524ff18-f17a-49f3-bcf8-ea22258834c3)
![Screenshot 2024-03-18 083757](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/f138df42-5ac2-499a-a44a-abbbcbf03bbf)

![Screenshot 2024-03-18 083816](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/301771e3-1e99-4cfd-af1a-f37483addff8)
![Screenshot 2024-03-18 083832](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/3278ff56-2715-492c-a3ac-15ce847f294b)

![Screenshot 2024-03-18 083844](https://github.com/JAIGANESHVETRISELVAN/exno1/assets/133752156/3c0f4daa-bea5-46e9-975b-2171150d1cc9)

# Result
Thus, the given data is read, cleansed and the cleaned data is saved into the file and the given data is read,remove outliers and save a new dataframe was created and executed successfully.
