Analysis of small data set using python, documenting step-by-step process of data analysis journey. 

The script below creates a DataFrame with hypothetical data containing only two columns: "Temperature" and "Sales". It then displays the first few rows, summary statistics, checks for missing values (none in this case), data types, and the correlation matrix between the variables.


# Step 1: Import necessary libraries
import pandas as pd

# Step 2: Load the dataset (hypothetical data)
data = {
    'Temperature': [25, 30, 35, 40, 45],
    'Sales': [100, 120, 140, 160, 180]
}
df = pd.DataFrame(data)

# Step 3: Explore the dataset
## Display the first few rows of the dataset
print("First few rows of the dataset:")
print(df.head())

## Summary statistics
print("\nSummary statistics:")
print(df.describe())

## Check for missing values
print("\nMissing values:")
print(df.isnull().sum())

## Data types of columns
print("\nData types of columns:")
print(df.dtypes)

# Step 4: Data Analysis
## Calculate correlations between variables
print("\nCorrelation matrix:")
print(df.corr())
