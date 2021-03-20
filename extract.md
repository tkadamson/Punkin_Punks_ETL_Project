## Extract

1. Loaded all csv's into Pandas DataFrames
2. Dropped all columns except the country name and the score. 
3. For the dataframes from the World Bank, we selected only the country name and 2019 data, effectively removing the other columns. 
4. Renamed the '2019' column to indicate which indicator we were working with in that dataframe.
5. Dropped all null values, since we only had the one column in each dataframe. 
6. Exported them as a csv back out the resources folder for next steps.
