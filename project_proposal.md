# Punkin_Punks_ETL_Project

### Project Proposal

For the ETL, we will use the 2019 data from the following datasets:
* World Happiness Report from the Sustainable Development Solutions Network: https://www.kaggle.com/unsdsn/world-happiness
* GDP per Capita (USD): https://data.worldbank.org/indicator/NY.GDP.PCAP.CD?view=chart
* Gross Savings (% of GDP): https://data.worldbank.org/indicator/NY.GNS.ICTR.ZS?view=chart
* Inflation, consumer prices (annual %): https://data.worldbank.org/indicator/FP.CPI.TOTL.ZG?view=chart

Once these are extracted and cleaned, we will use Jupyter Notebook to join the different metrics by country. The World Happiness index has the smallest number of countries, so we will only keep data for those countries and drop the rest from the World Bank.

After transforming these data into one dataframe, we will load it into a Mongo Database by country.

#### Timeline
The repo has already created with Thomas as the repo owner. 

Thomas will work on extracting the csv's and cleaning them in advance of Wednesday's class. Wednesday we'll work on the joining of the tables in Pandas and start the load process if there's time. Saturday we will finish the load process and clean up our repo and do a final report in the README. 
