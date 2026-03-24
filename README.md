# EXNO2DS
# AIM:
      To perform Exploratory Data Analysis on the given data set.
      
# EXPLANATION:
  The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.
  
# ALGORITHM:
STEP 1: Import the required packages to perform Data Cleansing,Removing Outliers and Exploratory Data Analysis.

STEP 2: Replace the null value using any one of the method from mode,median and mean based on the dataset available.

STEP 3: Use boxplot method to analyze the outliers of the given dataset.

STEP 4: Remove the outliers using Inter Quantile Range method.

STEP 5: Use Countplot method to analyze in a graphical method for categorical data.

STEP 6: Use displot method to represent the univariate distribution of data.

STEP 7: Use cross tabulation method to quantitatively analyze the relationship between multiple variables.

STEP 8: Use heatmap method of representation to show relationships between two variables, one plotted on each axis.

## CODING 
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("titanic_dataset.csv")
df
```
## Output
<img width="1642" height="572" alt="image" src="https://github.com/user-attachments/assets/5ac181aa-6dea-469d-9d56-21992e1d2e7e" />

## coding
```
df.info()
```
## output
<img width="537" height="468" alt="image" src="https://github.com/user-attachments/assets/e34f7b9e-6149-4915-aab4-c5d35c54db78" />

## coding
```
df.dtypes
```
## output
<img width="342" height="620" alt="image" src="https://github.com/user-attachments/assets/5c1bfe57-1fb6-40bd-b44f-c9d08d88ef5e" />

## CODING
```
df.value_counts()
```
## output 
<img width="1687" height="660" alt="image" src="https://github.com/user-attachments/assets/cb9436b8-0cb8-4972-ac7b-e78b8be2c320" />

## coding
```
df['Age'].value_counts()
```
## output
<img width="270" height="660" alt="image" src="https://github.com/user-attachments/assets/099e9fe2-3870-4b2c-9c9b-6c96db064c9f" />

## coding
```
corr = df.select_dtypes(include=np.number).corr()
sns.heatmap(corr,annot=True)
```

## output
<img width="796" height="613" alt="image" src="https://github.com/user-attachments/assets/02b3c93c-ef23-4a61-9686-f1ca84b94c10" />

# RESULT
Thus the dataset value is found
