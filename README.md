# Maryland Bills Analysis

An analysis of the 2019 Maryland General Assembly session.

Made by Jake Gluck [jagluck.github.io](jagluck.github.io).   
jakeagluck@gmail.com jagluck@terpmail.umd.edu

# Files

There are several files used in this analysis. They are all Jupyter Notebooks and they should be run in order. 

1. Create Dataset - This file pulls data from API and creates the bills dataset. 

2. Data Maniputlation - This file uses the bills dataset and more API calls to build the legislators and matrix datasets.  

3. Analysis - This file uses the three datasets to perform an analysis of the session. 

# Data

The project uses the Legiscan API. 

Find our data sets in the data folder. 

The main data sets used are: 

1. bills - Contains one row for each bill, including joint resolutions, and information about the bill. 

2. legislators - Contains one row for each legislator and information about what they did in the session. 

3. matrix - Contains the number of times different legislators co sponsored each other and the bill ids. This contains one row for each pair and in the name the legislators are ordered alphabetically.

# Graphics

The story has three D3 graphics:

1. A Saneky showing how bills progress through the session.

2. A force directed network showing co sponsorships in the House.

3.  A force directed network showing co sponsorships in the Senate.

# Config

This code gathers data using the Legiscan API.   
https://legiscan.com/legiscan

To use create a config file that contains your key for the API. 

It should look like this: 

```
{
    "legiscan_key" : "YOUR KEY HERE"
}
```
