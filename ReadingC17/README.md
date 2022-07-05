# Reading Class 17

## Web scraping

Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort. There are different ways to scrape websites such as online Services, APIs or writing your own code

## Is Web Scraping Legal?

Talking about whether web scraping is legal or not, some websites allow web scraping and some don’t. To know whether a website allows web scraping or not, you can look at the website’s “robots.txt” file. You can find this file by appending “/robots.txt” to the URL that you want to scrape.

or we can use <b>python code</b>  to check if a website allows web scraping or not we can use status_code as follows:

>> import requests

>> from bs4 import BeautifulSoup 

>> r=requests.get(" ENTER URL OF YOUR CHOICE")

>> r.status_code

The output to this should be 200. Anything other than 200 means that the website your trying to scrape either does not allow web scraping or allows partially.

## How Do You Scrape Data From A Website?
When you run the code for web scraping, a request is sent to the URL that you have mentioned. As a response to the request, the server sends the data and allows you to read the HTML or XML page. The code then, parses the HTML or XML page, finds the data and extracts it. 

To extract data using web scraping with python, you need to follow these basic steps:

- Find the URL that you want to scrape
- Inspecting the Page
- Find the data you want to extract
- Write the code
- Run the code and extract the data
- Store the data in the required format 

## Best Programming Language for Web Scraping
Obviously Python. There are so many diverse libraries you can use for web scraping. Some of them are:

- Selenium: 
This library uses Web Driver for Chrome in order to test commands and process the web pages to get to the data you need. 

- BeautifulSoup:
 Python library for pulling data out of HTML and XML files. It creates data parse trees in order to get data easily. 

- Pandas: 
Used for data extraction and manipulation. Usually, for databases, it saves data to a certain format.