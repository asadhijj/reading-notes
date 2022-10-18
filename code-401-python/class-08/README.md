# PANDAS 

* Pandas is an open source library in Python. It provides ready to use high-performance data structures and data analysis tools.
* Pandas module runs on top of NumPy and it is popularly used for data science and data analytics.
NumPy is a low-level data structure that supports multi-dimensional arrays and a wide range of mathematical array operations.
* Pandas has a higher-level interface. It also provides streamlined alignment of tabular data and powerful time series functionality.
* DataFrame is the key data structure in Pandas. It allows us to store and manipulate tabular data as a 2-D data structure.
* Pandas provides a rich feature-set on the DataFrame. For example, data alignment, data statistics, slicing, grouping, merging, concatenating data, etc.


**There are 3 data structures provided by the Pandas module, which are as follows:**


* Series: It is a 1-D size-immutable array like structure having homogeneous data.
* DataFrames: It is a 2-D size-mutable tabular structure with heterogeneously typed columns.
* Panel: It is a 3-D, size-mutable array.


**Pandas DataFrame**

DataFrame is the most important and widely used data structure and is a standard way to store data. DataFrame has data aligned in rows and columns like the SQL table or a spreadsheet database. We can either hard code data into a DataFrame or import a CSV file, tsv file, Excel file, SQL table, etc

Below is a short description of the parameters:

   * data - create a DataFrame object from the input data. It can be list, dict, series, Numpy ndarrays or even, any other DataFrame.
   * index - has the row labels
   * columns - used to create column labels
   * dtype - used to specify the data type of each column, optional parameter
   * copy - used for copying data, if any


There are many ways to create a DataFrame. We can create DataFrame object from Dictionaries or list of dictionaries. We can also create it from a list of tuples, CSV, Excel file, etc


## Inspecting data in DataFrame 

Running the DataFrame using its name displays the entire table. In real-time, the datasets to analyze will have thousands of rows. For analyzing data, we need to inspect data from huge volumes of datasets. Pandas provide many useful functions to inspect only the data we need. We can use df.head(n) to get the first n rows or df.tail(n) to print the last n rows.


1. **Getting Statistical summary of records**
We can get statistical summary (count, mean, standard deviation, min, max etc.) of the data using df.describe() function

2. **Sorting records**
We can sort records by any column using df.sort_values() function

3. **Slicing records**
It is possible to extract data of a particular column, by using the column name.
It is also possible to slice multiple columns. This is done by enclosing multiple column names enclosed in 2 square brackets, with the column names separated using commas.
It is also possible to slice rows. Multiple rows can be selected using “:” operator


4. **Filtering data**
It is also possible to filter on column values,Any comparison operator can be used to filter, based on a condition
Another way to filter data is using the 'isin'



5. **Rename column**
It is possible to use the df.rename() function to rename a column. The function takes the old column name and new column name as arguments

6. **Data Wrangling**
Data Science involves the processing of data so that the data can work well with the data algorithms. Data Wrangling is the process of processing data, like merging, grouping and concatenating. The Pandas library provides useful functions like merge(), groupby() and concat() to support Data Wrangling tasks.


## Create a DataFrame by passing Dict of Series

To create a Series, we can use the pd.Series() method and pass an array to it


## Column Selection, Addition, Deletion

It is possible to select a specific column from the DataFrame.

It is also possible to add columns to an existing DataFrame

We can delete columns using the `delete` and `pop` functions




***

## Sources 

[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[Pandas Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)

[Pandas Tutorials](https://realpython.com/learning-paths/pandas-data-science/)

[Master Pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)


***


## Things i want to know more about 

usage of pandas with real world problems
