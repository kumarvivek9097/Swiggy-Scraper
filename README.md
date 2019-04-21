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
- time

## About the code
The whole project is divided into two part:
  - Crawler: It will crawl the entire website and fetch required links i.e url of each restaurant.
  - Scraper: It will take each links fetched from crawler as input and will go to each page to extract the required information.
  
### Techniques used

- Headers:  Python Requests does not force you to use request headers while sending requests but there are few smart websites that does not let you to extract any data without certain headers. So it is always good to set headers.

- Time Delay: A delay of 5 seconds has been given after each url hit to prevent scraper from being blocked.

- Multiprocessing: As there are more than 57,000 restaurants listed on swiggy so extracing data from each url with a delay of 5 second will take very long time. So to overcome this multiprocessing is used to speed up scraping. 
