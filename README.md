# Ex03-Univariate-Analysis
# Aim
To read the given data and perform the univariate analysis with different types of plots
# Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Algorithm
# Step1
Read the given data.

# Step2
Get the information about the data.

# Step3
Remove the null values from the data.

# Step4
Mention the datatypes from the data.

# Step5
Count the values from the data.

# Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.
# Program
```
# Developed by        : KIRUTHIKA S
# Registration Number : 212221040085
```
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
# OUTPUT
# DATA

![image](https://user-images.githubusercontent.com/128348968/228207481-02c009b9-9f59-475f-b03b-4dd1b27aefbf.png)
# DATA HEAD
![image](https://user-images.githubusercontent.com/128348968/228208440-cf456f2d-b816-4b66-85cb-107d9b21d1d6.png)
# DATA INFORMATION
![image](https://user-images.githubusercontent.com/128348968/228208720-38fa59d7-3cdf-4aab-b65a-6bedee205e9a.png)
# DATA DESCRIBE
![image](https://user-images.githubusercontent.com/128348968/228208932-140778b6-3341-401d-a92f-c717c1eabd0c.png)
# DATA NULL VALUES
![image](https://user-images.githubusercontent.com/128348968/228209067-3e5e083b-3d1a-47ec-9aa1-6efba4251152.png)
# DATA'S DATATYPES
![image](https://user-images.githubusercontent.com/128348968/228209275-b097e8a7-c081-4f7a-973e-506f797659bf.png)
# DATA'S VALUECOUNT
![image](https://user-images.githubusercontent.com/128348968/228209438-9245f166-d147-438b-aeb2-208c18fe79b0.png)
# BOXPLOT
![image](https://user-images.githubusercontent.com/128348968/228209573-b9b47934-691e-4abb-8091-fc29a1b8c576.png)
# COUNTPLOT
![image](https://user-images.githubusercontent.com/128348968/228209740-c6b7c37f-32a8-4f29-ab9d-499e368eefd9.png)
# DISTRIBUTION PLOT
![image](https://user-images.githubusercontent.com/128348968/228209859-d77fd3a0-06d8-4173-aa92-cee922a9cc05.png)
# HISTOGRAM PLOT
![image](https://user-images.githubusercontent.com/128348968/228210336-0fbc274e-9f75-4f87-99af-290b5ffaa4e1.png)
# Result
Thus we have read the given data and performed the univariate analysis with different types of plots.



