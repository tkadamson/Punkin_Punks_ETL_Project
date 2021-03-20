# Punkin_Punks_ETL_Project

Here is the description for our ETL Project on happiness data and other world data:

## Extract

1) Loaded all csv's into Pandas DataFrames

2) Dropped all columns except the country name and the score.
 
3) For the dataframes from the World Bank, we selected only the country name and 2019 data, effectively removing the other columns. 

4) Renamed the '2019' column to indicate which indicator we were working with in that dataframe.

5) Dropped all null values, since we only had the one column in each dataframe. 

6) Exported them as a csv back out the resources folder for next steps.


## Transform

1) Tables were cleaned so they would be concise.
    * Clean_Happiness, which has Country Name and Happiness Rank.
    * Clean_GDP, which has the Country Name and Gross Domestic Product (GDP)
    * Clean_Inflation, which has the Country Name and Inflation Rate
    * Clean_Savings, which has the Country Name and the Savings Rate

2) The cleaned tables were converted into dataframes

3) The dataframes were joined into one large table, **World_Well_Being**, through multiple left joins.
    
4) The World_Well_Being table was exported into a csv file.


## Load to Mongo

Steps taken to load transformed data to a Mongo Database

1) Import dependencies into Jupyter Notebook
    * pymongo
    * pandas as pd
    
2) Read in the transformed clean csv file from the Transform step

3) Connect to our MongoDB, create a database and declare the collection

4) Create a for loop to itterate through the rows of data in the csv and load each row to our Mongo Database

5) Verify our results are in the Mongo Database

