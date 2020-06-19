# Exploration and Analysis of Darknet Markets
## Aim
This project aims to create a useful database consisting of historical data from multiple darknet sites. Of particular interest is pricing variation over time, the impact of geography on the availability and cost of goods and if distribution of products are controlled by a small number of sellers or widely dispersed within a given region.
## Data
The raw data was scraped from a collection of darknet markets by Gwern (https://www.gwern.net/DNM-archives) between 2013 and 2015. Information extracted includes all listing information (Title, Seller Name, Price and in some cases ratings). Based on Bitcoin/ other currency cost and the date of the scrape we can normalise the value per lisiting in USD.

## Storing Cleaned Data
Once data is made to an acceptable standard it is added to a database hosted on Amazon RDS.

## Status
The database currently contains approximately 400,000 listings from two of the largest darknet markets, Silkroad2 (Now shut down) and Hydra (One of the largest markets, primarily servicing the former USSR). Data from Dreammarket will be added soon.

## Future Direction
I've been working on a webscraper to allow for comparison of historical data and recent listings and hope to have this operational shortly.

### File Info:
ConvertFilesToHTML contains a script to make the scraped files readable as HTML files //
The Cryptomarket files contain functions to extract data of interest and some preliminary cleaning //
masterdarknet.xlsx is the master dataframe //
darknet_1 features code to merge and standardise the data from the different markets including checking for inconsistencies and further cleaning. Currently working on a Dash app to display summary statistics by market.
