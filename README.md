# Ex-09-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.
# CODE
```
#DEVELOPED BY : Akshayaa M
#REGISTER NUMBER: 212222230009
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
tips_df=sns.load_dataset("tips")
tips_df
sns.barplot(data = tips_df,x = "total_bill",y = "day")
sns.relplot(data = tips_df,x = "total_bill", y="tip",hue = "smoker", style = "smoker")
sns.displot(data = tips_df,x = "total_bill", y="tip",hue = "smoker")
sns.barplot(data = tips_df,x = "total_bill", y="tip",hue = "smoker")
sns.kdeplot(data = tips_df, x ="total_bill", y = "tip", size ="size")
sns.relplot(data = tips_df, x ="total_bill", y = "tip", hue = "day", col = "time")
sns.relplot(data = tips_df, x = "total_bill",y = "tip", col="day",col_wrap=2)
sns.lineplot(x = "total_bill", y = "tip", data = tips_df, hue = "sex",
style = "sex",
markers = ["o","<"], legend = "auto")
```
# OUPUT
![EX-09-DATA-VISUALIZAION_1](1.png)
![EX-09-DATA-VISUALIZAION_1](2.png)
![EX-09-DATA-VISUALIZAION_1](3.png)
![EX-09-DATA-VISUALIZAION_1](4.png)
![EX-09-DATA-VISUALIZAION_1](5.png)
![EX-09-DATA-VISUALIZAION_1](6.png)
![EX-09-DATA-VISUALIZAION_1](7.png)
![EX-09-DATA-VISUALIZAION_1](8.png)
![EX-09-DATA-VISUALIZAION_1](9.png)
# RESULT
Thus Data Visualization is performed on the given dataset and save the data to a file. 