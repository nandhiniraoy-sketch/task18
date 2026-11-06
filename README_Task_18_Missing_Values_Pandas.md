# Task 18 - Missing Values in Pandas

## Objective

Learn how to identify and handle missing values using Pandas.

## Requirements

-   Python
-   Pandas
-   Jupyter Notebook

## Programs

### 1. Import Pandas

``` python
import pandas as pd
```

### 2. Create Dataset

``` python
data={"Name":["Ram","Sita","John","Anu"],"Age":[21,None,23,22],"Marks":[85,90,None,88]}
df=pd.DataFrame(data)
print(df)
```

### 3. Check Missing Values

``` python
print(df.isna())
```

### 4. Count Missing Values

``` python
print(df.isna().sum())
```

### 5. Check Non-Missing Values

``` python
print(df.notna())
```

### 6. Remove Missing Values

``` python
print(df.dropna())
```

### 7. Fill Missing Values with 0

``` python
print(df.fillna(0))
```

### 8. Fill Age with Mean

``` python
df["Age"]=df["Age"].fillna(df["Age"].mean())
print(df)
```

### 9. Fill Marks with Median

``` python
df["Marks"]=df["Marks"].fillna(df["Marks"].median())
print(df)
```

### 10. Final Cleaned Dataset

``` python
df["Age"]=df["Age"].fillna(df["Age"].mean())
df["Marks"]=df["Marks"].fillna(df["Marks"].median())
print(df)
```

## Concepts Used

-   NaN
-   isna()
-   notna()
-   isna().sum()
-   dropna()
-   fillna()
-   mean()
-   median()

## Outcome

Successfully identified, counted, removed, and filled missing values to
create a cleaned dataset.
