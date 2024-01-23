## Class 12 Notes

1. **Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?**

    - Pandas is a library that houses many tools and data that is widely used in data science, analytics and machine learning tasks, some functionality and operations are:

        ### Functionalities

        - **Data Manip and Cleaning** - Pandas provides functions and methods to reshape, sort, merge and summarize datasets. Very useful for transforming data into a certain format

        - **Data Analysis** - enables computation of mean, median, mode, variance and more. Useful for exploratory data analysis and understanding data trends.

        - **Data Representation** - offers comprehensive tools for readable and concise data representation, which is crucial for interpreting and examining data effectively.

        ### Operations

        -**Data Merging** - combining different datasets through various types of concatenation

        - **Data Filtering** - apply conditions to filter data using functions to change the datasets.

        - **Time Series Analysis** - able to handle and manipulate time-series data for many applications.

2. **What are the primary data structures in Pandas, and how do they differ in terms of use cases?**

    - **Series** - One dimensional arrays-like objects that contain data and labels associated with the data called index. These are more used in single columns on a datasheet.

    - **Dataframes** - Two dimensional arrays that are size-mutable that could have tabular data structures with labels(rows and columns). More suited for real-world applications such as excel and SQL.

3. **Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?**

    - Pandas can read in common file formats such as:
        - CSV(`read_csv`), `pandas.read_csv(filepath)`
        - Excel(`read_excel`), `pandas.read_excel(filepath)`
        - JSON(`read_json`), `pandas.read_json(filepath)`
        - SQL Database(`read_SQL`), `pandas.read_SQL(filepath)`


```
import pandas as pd

# Loading an Excel file into a DataFrame
my_excel = pd.read_excel('file.excel')

# Viewing the first few rows of the DataFrame
print(df.head())
```
