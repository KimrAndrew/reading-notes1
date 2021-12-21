# Web Scraping With Python In 4 minutes

## Web Scraping

  - technique to automatically access and extract large amounts of information from a website

## Important notes about web scraping:

  1. Read through the website's Terms and Conditions, most sites prohibit you from using the data for commercial purposes
  2. Make sure you are not downloading data too rapidly

## Python Code

import the following libraries

``` python
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

url = #url
response = response.get(url)
```
parse the html with BeautifulSoup

``` python
soup = BeautifulSoup(response.text, 'html.parser')
soup.findAll('a')
```

make sure to set a timeout to help avoid gettign flagged as a spammer
