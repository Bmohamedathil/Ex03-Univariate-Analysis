# Ex03-Univariate-Analysis
## Aim :

To read the given data and perform the univariate analysis with different types of plots.

## Explanation :

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm:

### Step1:

Read the given data.

### Step2:

Get the information about the data.

### Step3:

Remove the null values from the data.

### Step4:

Mention the datatypes from the data.

### Step5:

Count the values from the data.

### Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program:
```
Developed By : B.Mohamed Athil
Register Number : 212222230081



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
## Output :

### Dataset :

![image](https://user-images.githubusercontent.com/119560261/228605224-9c3d760d-074e-42a8-9f28-b4f93fad5b1c.png)

### Head :

![image](https://user-images.githubusercontent.com/119560261/228605609-21e81472-8805-42a2-a058-acacb22f2ef2.png)

### Info :

![image](https://user-images.githubusercontent.com/119560261/228605819-bbf22fec-d144-43a3-a533-79d2513eb40a.png)

### Describe :

![image](https://user-images.githubusercontent.com/119560261/228605924-eaa7b1ec-9ac7-4cfb-b2e2-ad4e85a33b8f.png)

### Isnull :

![image](https://user-images.githubusercontent.com/119560261/228606225-ae4d45c1-224d-4cd0-be96-1adf12a40c71.png)

### dtypes :

![image](https://user-images.githubusercontent.com/119560261/228606419-c0fb766b-ae2e-41db-a281-2a052ba2803a.png)

### Valuecount :

![image](https://user-images.githubusercontent.com/119560261/228606529-271948a9-3c12-4d20-b5b1-572bdb49159f.png)

### Boxplot :

![image](https://user-images.githubusercontent.com/119560261/228606632-ac3991b0-8a93-4e45-851b-6d6040c3b0f9.png)

### Countplot :

![image](https://user-images.githubusercontent.com/119560261/228606758-3f635384-627a-4a60-991a-d269602f2a49.png)

### Distribution plot :

![image](https://user-images.githubusercontent.com/119560261/228607016-c284a541-6eb8-4d02-bd68-5d346faacb84.png)

### Histogram plot :

![image](https://user-images.githubusercontent.com/119560261/228607109-2d72b5c9-3d0f-46a0-aa2c-1016b1bd30cd.png)

# Result :

Thus we have read the given data and performed the univariate analysis with different types of plots.









