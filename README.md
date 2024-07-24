# Amazon Product Scraper

This Python script scrapes product information from Amazon's search results page for "formal shoes for men". It extracts product titles, prices, and URLs, and saves the data to a CSV file.

## Script Overview

The script performs the following tasks:

### Send HTTP Request

Fetches the search results page from Amazon for "formal shoes for men".

### Parse HTML

Uses BeautifulSoup to parse the HTML content of the page.

### Extract Links

Finds and constructs full URLs for product pages from the search results.

### Scrape Product Details

For each product page, extracts the title and price.

### Save to CSV

Compiles the data into a DataFrame and saves it to a CSV file named `amazon_data.csv`.

## Code Details

### Functions

- **`get_title(soup)`**: Extracts the product title from the HTML content.
- **`get_price(soup)`**: Extracts the product price from the HTML content.

### Main Execution

- **Set Headers**: Configures the HTTP headers to mimic a real browser.
- **Fetch Search Results**: Requests the search results page from Amazon.
- **Extract Product Links**: Finds and builds links to individual product pages.
- **Scrape Product Pages**: Requests each product page and extracts the title and price.
- **Handle Exceptions**: Handles HTTP errors and continues processing.
- **Save Data**: Writes the data to a CSV file.

## Requirements

- Python 3.x
- Requests library
- BeautifulSoup4 library
- pandas library
- numpy library

You can install the required libraries using pip:

```bash
pip install requests beautifulsoup4 pandas numpy
```
