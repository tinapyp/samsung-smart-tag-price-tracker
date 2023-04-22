# Amazon_Page_Scraper
Building Amazon Page Scraper using Python

This script is a web scraper that checks the price of a Samsung SmartTag Bluetooth Tracker on Amazon and adds the data to a CSV file. The script uses the BeautifulSoup library to parse the HTML of the Amazon product page, and the Requests library to make a request to the webpage.

Syntax and Functions
The following libraries are imported in the script:

javascript
Copy code
from bs4 import BeautifulSoup
import requests
import datetime
import csv
import time
import pandas as pd
The check_price() function is used to scrape the price of the Samsung SmartTag Bluetooth Tracker on Amazon, and add the data to a CSV file. The function performs the following steps:

Connect to the Amazon product page and pull in the data using requests.
Parse the HTML using BeautifulSoup.
Find the product title and price on the webpage.
Clean the data by stripping unnecessary whitespace and characters.
Add the current date to the data.
Write the data to a CSV file using the csv library.
The function is run every 20 seconds using a while loop:

scss
Copy code
while(True):
    check_price()
    time.sleep(20)
This loop ensures that the price is checked and added to the CSV file every 20 seconds.

Finally, the pandas library is used to read the data from the CSV file:

python
Copy code
pd = pd.read_csv(r'C:\Users\Fathin Afif\Python Learning\Projects\AmazonShirtPageWebScraper.csv')
This line of code can be used to monitor the data that has been scraped from the Amazon product page.
