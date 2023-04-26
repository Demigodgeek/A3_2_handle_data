# Dollars and Change

In this activity, you'll prepare and clean data by removing symbols in the dataset, converting data types, filling in missing values, and dropping any duplicate data.

Instructions:

1. Import the Pandas and `pathlib` libraries.

2. Use `Path` with the `read_csv` function to read the CSV file into the DataFrame. Use the `index_col`, `parse_dates`, and `infer_datetime_format` parameters to set the Date column as the index.

3. Confirm the import by using the `head` function to review the first five rows of the DataFrame .

4. Use the `dtypes` function to check the data types of the DataFrame, and identify the ones that are strings.

5. Use the `str.replace` function to replace all the dollar signs in the Total Payments column. Then review the first five rows of the DataFrame to confirm the update.

6. Use the `astype` function to change the data type of the Total Payments column from `object (string)` to `float`. Then call the `dtypes` function on the DataFrame to confirm the update.

7. For the Profit Margin column, remove all the percent signs and convert the data types to `float` by repeating the preceding steps. Call the `dtypes` function on the DataFrame to confirm the update.

8. Use the `isnull` function along with the `sum` function to determine the number of missing values in the DataFrame.

9. Use the `fillna` function to fill any missing values in just the Profit Margin column with the value of 0. Then rerun the `isnull().sum()` function to confirm that you handled missing values.

10. Use the Pandas `duplicated` function along with the `sum` function to determine the number of duplicated entries in the DataFrame.

11. Use the Pandas `drop_duplicates` function to remove all duplicated entries. Review the first 10 rows of the DataFrame to confirm the update.


References:

[Pandas read_csv function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html)

[Pandas dtypes function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.dtypes.html)

[Pandas str.replace function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.str.replace.html)

[Pandas astype funtion](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.astype.html)

[Pandas isnull function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.isnull.html)

[Pandas duplicated function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.duplicated.html)