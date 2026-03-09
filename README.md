# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# NAME : MADHAVAN K

# REG NO : 212224220054

# REF NO : 24901129

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
# STEP 1: Include the necessary Library

import pandas as pd
import matplotlib.pyplot as plt

%matplotlib inline
```
```
# STEP 2: Read the given Data

heights = pd.read_csv("heights.csv")
heights.head()
```
```
# STEP 3,4,5: Apply visualization

plt.figure()
plt.bar(heights.iloc[:,0], heights.iloc[:,1])
plt.xlabel("Category")
plt.ylabel("Height")
plt.title("Bar Chart of Heights")
plt.xticks(rotation=45)
plt.show()
```

```
iris = pd.read_csv("iris.csv")
iris.head()
```
```
plt.figure()
plt.scatter(iris.iloc[:,0], iris.iloc[:,2])
plt.xlabel("Sepal Length")
plt.ylabel("Petal Length")
plt.title("Scatter Plot - Iris Dataset")
plt.show()
```

```
loan = pd.read_csv("Loan_data.csv")
loan.head()
```
```
# Read the data
loan = pd.read_csv("Loan_data.csv")

# Check column names
print(loan.columns)

# Select numeric column properly
numeric_column = loan.select_dtypes(include=['int64', 'float64']).columns[0]

# Remove missing values
loan_clean = loan[numeric_column].dropna()

# Plot Histogram
plt.figure()
plt.hist(loan_clean, bins=10)
plt.xlabel(numeric_column)
plt.ylabel("Frequency")
plt.title("Histogram of Loan Data")
plt.show()
```
```
dataset = pd.read_csv("Data_set.csv")
dataset.head()
```

```
plt.figure()
plt.scatter(dataset_clean.iloc[:,0], dataset_clean.iloc[:,1])
plt.xlabel("X Values")
plt.ylabel("Y Values")
plt.title("Scatter Plot of Dataset")
plt.show()
```
```
sample = pd.read_csv("SAMPLEIDS.csv")
sample.head()
```

```
plt.figure()
plt.pie(sample.iloc[:,1], labels=sample.iloc[:,0], autopct='%1.1f%%')
plt.title("Pie Chart Representation")
plt.show()
```
<img width="1377" height="1024" alt="Screenshot 2026-02-26 093301" src="https://github.com/user-attachments/assets/c9c0d874-641b-4121-81e4-fd3beec1c174" />

<img width="1472" height="1018" alt="Screenshot 2026-02-26 093316" src="https://github.com/user-attachments/assets/bafef6ed-d657-4796-992e-0dc32d8a6cb4" />

<img width="1438" height="1006" alt="Screenshot 2026-02-26 093334" src="https://github.com/user-attachments/assets/fe581ff0-87f5-4969-94be-a97055aba145" />

<img width="1343" height="1012" alt="Screenshot 2026-02-26 093354" src="https://github.com/user-attachments/assets/c3837227-106e-41fe-b86a-c08e2cc63745" />


# Result:

Thus, Data Visualization using matplotlib python library for the given datasets has been successfully performed.
