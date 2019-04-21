# Swiggy Scraper
A Scraping project to scrape restaurant information from [Swiggy](https://www.swiggy.com).  This scraper is able to scrape data for entire Indian restaurants.

## Data
The links of all the restaurants can be find in links.csv file and scraped data can be found in scrape_data.csv file.
The following variables are saved:

- `Restaurant Name`: Name of the restaurant
- `Longitude`: Longitude coordinate of the restaurant's location
- `Latitude`: Latitude coordinate of the restaurant's location
- `Price For Two`: Cost for two in rupees
- `Region`: Region where restaurant is located
- `Rating`: Average rating out of 5

## Libraries 
Following libraries are used in this project:

- BeautifulSoup
- requests
- re
- json
- pandas
