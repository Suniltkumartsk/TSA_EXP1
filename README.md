# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 19.08.25 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
# NAME: SUNIL KUMAR T
# REG: 212223240164

import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("usedcars.csv")

# Group by Year and calculate average kilometers driven
yearly_data = df.groupby("Year")["Kilometers_Driven"].mean().reset_index()

# Plot
plt.figure(figsize=(8,5))
plt.plot(yearly_data["Year"], yearly_data["Kilometers_Driven"], marker='o', linestyle='-', color='g')

plt.title("Average Kilometers Driven by Year of Manufacture")
plt.xlabel("Year")
plt.ylabel("Average Kilometers Driven")
plt.grid(True)
plt.show()

```









# OUTPUT:
<img width="814" height="476" alt="Screenshot 2025-08-19 205148" src="https://github.com/user-attachments/assets/796e573e-1686-4316-8c32-7b62b9c9ccc9" />






# RESULT:
Thus we have created the python code for plotting the time series of given data.
