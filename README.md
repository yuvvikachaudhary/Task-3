# Task-3

import pandas as pd
import matplotlib.pyplot as plt
import numpy as np

# Create sample data
data = {
    'Category': ['A', 'B', 'C', 'D', 'E'],
    'Value1': [23, 45, 56, 78, 33],
    'Value2': [12, 33, 44, 55, 22]
}

df = pd.DataFrame(data)

# Bar Chart
plt.figure(figsize=(8, 6))
plt.bar(df['Category'], df['Value1'], color='skyblue', label='Value1')
plt.xlabel('Category')
plt.ylabel('Values')
plt.title('Bar Chart: Values by Category')
plt.legend()
plt.show()

# Line Chart
plt.figure(figsize=(8, 6))
plt.plot(df['Category'], df['Value1'], label='Value1', color='green', marker='o')
plt.plot(df['Category'], df['Value2'], label='Value2', color='orange', marker='s')
plt.xlabel('Category')
plt.ylabel('Values')
plt.title('Line Chart: Values by Category')
plt.legend()
plt.show()
