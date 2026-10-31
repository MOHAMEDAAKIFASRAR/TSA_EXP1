# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 31/10/2026

# AIM:
To develop a Python program to plot the time series data using the AirPassengers dataset and visualize the changes in the number of air passengers over time.
### Dataset Name : AirPassengers
# ALGORITHM:
1. Import the required packages such as Pandas and Matplotlib.
2. Read the AirPassengers dataset using Pandas.
3. Convert the Month column into datetime format.
4. Select the Month and Passengers columns from the dataset.
5. Plot the time series data using a line graph.
6. Add a suitable title, X-axis label, Y-axis label and grid.
7. Display the graph.

# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv('/content/AirPassengers.csv')

df['Month'] = pd.to_datetime(df['Month'])

plt.figure(figsize=(10, 5))

plt.plot(df['Month'], df['#Passengers'],
         color='blue', linewidth=1.8)

plt.title('Air Passengers Over Time')
plt.xlabel('Year')
plt.ylabel('Number of Passengers')

plt.grid(True, alpha=0.3)

plt.tight_layout()
plt.show()
```


# OUTPUT:
<img width="782" height="377" alt="image" src="https://github.com/user-attachments/assets/11b394e1-b96f-4d8f-90eb-fe3a79f84449" />


# RESULT:
Thus, we have successfully created and executed a Python program to plot the time series data using the AirPassengers dataset. The graph clearly represents the changes in the number of air passengers from 1949 to 1960.
