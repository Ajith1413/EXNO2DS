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

## CODING AND OUTPUT
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("/content/titanic_dataset.csv")
df
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/4069d465-7163-4516-959e-a5927d7ed43f)
```
df.info()
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/336e313e-86ed-4ca9-8d6f-12c11c021a96)

```
df.shape
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/e2f8a0d5-e4d7-4242-8897-135b7ba283a5)
```
import pandas as pd
df=pd.read_csv("/content/titanic_dataset.csv")
df.set_index("PassengerId",inplace=True)
print(df.set_index)
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/9d5717de-831f-47bc-b1b2-8397289f3a48)
```
df.describe()
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/f9bc25c7-4d5e-447b-8fb0-918df31c3f1c)
```
df.nunique()
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/1b777e29-4a91-45f3-89fc-253bbce4ed09)
```
df["Survived"].value_counts()
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/55e4fb63-ee1a-4172-8b86-d2b627f2e660)
```
per=(df["Survived"].value_counts()/df.shape[0]*100).round(2)
per
```
![image](https://github.com/Ajith1413/EXNO2DS/assets/139842524/7c58eb4c-b52d-4082-bd8d-f590caec9095)




# RESULT
        <<INCLUDE YOUR RESULT HERE>>
