# Experiment 2: Data Visualization Using Matplotlib and Seaborn

## Aim

To visualize data using Matplotlib and Seaborn libraries.

## Algorithm

1.  **Start.**
2.  Import the Matplotlib and Seaborn libraries.
3.  Load data into a Pandas DataFrame.
4.  Plot a histogram for age distribution using `plt.hist()`.
5.  Plot a scatter plot for Age vs. Salary using `sns.scatterplot()`.
6.  Plot salary distribution using `sns.boxplot()`.
7.  Show the plots sequentially.
8.  **Stop.**


## Program

# Step 1: Import the required libraries

import numpy as np

import pandas as pd

import matplotlib.pyplot as plt

import seaborn as sns

# Step 2: Create a dataset
data = {
    'Age': [22, 25, 28, 30, 35, 40, 45, 50],
    'Salary': [20000, 25000, 30000, 35000,
               40000, 45000, 50000, 60000]
}

# Step 3: Convert data into DataFrame

df = pd.DataFrame(data)

# Step 4: Plot histogram for Age distribution

plt.hist(df['Age'], bins=5, color='skyblue', edgecolor='black')

plt.title('Age Distribution')

plt.xlabel('Age')

plt.ylabel('Frequency')

plt.show()

# Step 5: Plot scatter plot for Age vs Salary
sns.scatterplot(x='Age', y='Salary', data=df)

plt.title('Age vs Salary')

plt.xlabel('Age')

plt.ylabel('Salary')

plt.show()

# Step 6: Plot boxplot for Salary distribution
sns.boxplot(y=df['Salary'])

plt.title('Salary Distribution')

plt.ylabel('Salary')

plt.show()

## output

<img width="1920" height="1619" alt="image" src="https://github.com/user-attachments/assets/cc518d93-053b-4f12-b645-967001c555a9" />


## result

Thus, data visualization was successfully performed using Matplotlib and Seaborn libraries. Histogram, scatter plot, and box plot were created to analyze age distribution, the relationship between age and salary, and salary distribution.
