## Load data to MongoDB

Steps taken to load transformed data to a Mongo Database

1) Import dependencies into Jupyter Notebook
    * pymongo
    * pandas as pd
    
2) Read in the transformed clean csv file from the Transform step

3) Connect to our MongoDB, create a database and declare the collection

4) Create a for loop to itterate through the rows of data in the csv and load each row to our Mongo Database

5) Verify our results are in the Mongo Database
