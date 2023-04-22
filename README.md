# Amazon_Page_Scraper
Building Amazon Page Scraper using Python

This is a Python code for web scraping Amazon website to extract the price and title of a product and write the data into a CSV file. The code is also set to run the web scraping function every 20 seconds using a while loop. Finally, the code uses the Pandas library to read the CSV file for monitoring the data.

Here's a breakdown of the code:

The required libraries are imported at the beginning of the code:

BeautifulSoup: A Python library for pulling data out of HTML and XML files.
requests: A Python library for making HTTP requests.
datetime: A Python module for working with dates and times.
csv: A Python module for working with CSV files.
time: A Python module for working with time.
pandas: A Python library for data manipulation and analysis.
A function named check_price() is defined, which contains the web scraping code to extract the product's price and title from Amazon's website. The function adds the data into a CSV file.

The function check_price() is called using a while loop that runs indefinitely. The function is set to execute every 20 seconds using the time.sleep(20) method.

Finally, the code uses the Pandas library to read the CSV file and monitor the data.

Note that the code is specific to scraping the price and title of a Samsung SmartTag Bluetooth Tracker Locator product from Amazon's website. If you want to scrape data for a different product, you'll need to modify the code accordingly.
