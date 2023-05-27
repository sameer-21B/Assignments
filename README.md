# PandasAssignment

Q1. How do you load a CSV file into a Pandas DataFrame?
--- use pandas.read_csv() function to load csv file into a pandas dataframe.

Q2. How do you check the data type of a column in a Pandas DataFrame?
--- we can check the data type of a column in pandas using dtype attribute of pandas dataframe.

Q3. How do you select rows from a Pandas DataFrame based on a condition?
--- dataframe[dataframe.column > value]

Q4. How do you rename columns in a Pandas DataFrame?
--- dataframe.rename(columns={'oldvalue':'newvalue'},inplace=True)

Q5. How do you drop columns in a Pandas DataFrame?
--- dataframe.drop(['column'],axis=1,inplace=True)

Q6. How do you find the unique values in a column of a Pandas DataFrame?
--- dataframe['column'].unique()

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
--- dataframe.isna().sum()

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
--- dataframe['column_name'].fillna(value,inplace=True)

Q9. How do you concatenate two Pandas DataFrames?
--- pd.concat([dataframe1,dataframe2],axis=0)

Q10. How do you merge two Pandas DataFrames on a specific column?
--- dataframe1.merge(dataframe2,how="right")

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
--- da[['Month','SalesAmount']].groupby(['Month']).sum()

Q12. How do you pivot a Pandas DataFrame?
--- da.pivot('index_col','column_label_col','value_col')

Q13. How do you change the data type of a column in a Pandas DataFrame?
--- dataframe.astype({'colname1':'datatype'})

Q14. How do you sort a Pandas DataFrame by a specific column?
--- dataframe.sort_values("column_name")

Q15. How do you create a copy of a Pandas DataFrame?
--- dataframe.copy()

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
--- data[(data["colname1"]==value1) & (data["colname2"]>value2)]

Q17. How do you calculate the mean of a column in a Pandas DataFrame?
--- dataframe["column_name"].mean()

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
--- dataframe["column_name"].std()

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
--- data["colname1"].corr(data["colname2"])

Q20. How do you select specific columns in a DataFrame using their labels?
--- dataframe[["colname1","colname2"]]

Q21. How do you select specific rows in a DataFrame using their indexes?
--- dataframe.iloc[idx1:idx2]

Q22. How do you sort a DataFrame by a specific column?
--- dataframe.sort_values("column_name")

Q23. How do you create a new column in a DataFrame based on the values of another column?
--- dataframe['new_col']=da['colname']+3

Q24. How do you remove duplicates from a DataFrame?
--- Using the dataframe.drop_duplicates() method.

Q25. What is the difference between .loc and .iloc in Pandas?
--- a.) The loc() function is label based data selecting method which means that we have to pass the name of the row or column which we want to select 
	whereas the iloc() function is index based selecting method.
    b.) loc() function includes the last value passed in the range whereas iloc() doesn't.
    c.) loc() can accept boolean data whereas iloc() can't.
    d.) loc() can be used to perform many operations on the sliced dataframe whereas iloc() can't be used for performing any operations.
