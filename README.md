# Exploration and analysis of Darknet Markets
## Data
The raw data was scraped from a collection of darknet markets by Gwern (https://www.gwern.net/DNM-archives) between 2013 and 2015. Information extracted includes all listing information (Title, Seller Name, Price and in some cases ratings). Based on Bitcoin/ other currency cost and the date of the scrape we can normalise the value per lisiting in USD.

## Storing Cleaned Data
Once data is made to an acceptable standard it is added to a database hosted on Amazon RDS.

## Future Direction
I've been working on a webscraper to allow for comparison of historical data and recent listings and hope to have this operational shortly.
