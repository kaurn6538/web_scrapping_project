## Web Scraping Project
This project demonstrates how to scrape data from a real website using Python, specifically the BeautifulSoup and Requests libraries. The scraped data is processed into a pandas DataFrame and then exported to a CSV file.

## Table of Contents
Installation
Usage
Project Structure
Code Overview
Output
License
Installation

## Clone the repository:


*     git clone https://github.com/kaurn6538/web_scraping_project.git
cd web-scraping-project

## Install the required Python libraries:


*     pip install requests beautifulsoup4 pandas

## Usage
Specify the URL: The script uses the URL of the webpage containing the table data.

## Run the script:


python scraper.py
Check the output: The data will be saved as a CSV file in the specified directory.



*    requests: To send HTTP requests to the web page.
*    BeautifulSoup: To parse the HTML and extract the required data.
*    pandas: To handle data manipulation and export it to a CSV file.

## Sending HTTP Request:

The script sends a request to the website using the requests.get() method.

## Parsing the HTML:

The HTML content is parsed using BeautifulSoup.

The specific table is located using soup.find_all('table')[1], or by specifying the class.

## Extracting Table Headings:

Table headings are extracted with table.find_all('th').
A list comprehension is used to clean and store these headings.

## Extracting Row Data:

Each row's data is extracted, cleaned, and appended to the pandas DataFrame.
Exporting to CSV:

The DataFrame is exported to a CSV file using df.to_csv().

## Output
The script generates a CSV file containing the scraped data, saved to the specified directory.

