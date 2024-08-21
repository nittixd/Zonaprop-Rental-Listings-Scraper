# Zonaprop Rental Listings Scraper

This project is a Python-based web scraper designed to extract detailed information from rental property listings on Zonaprop. The scraper gathers data such as prices, expenses, descriptions, addresses, and images, and stores it in a structured CSV file for further analysis.

## Project Overview

The Zonaprop Rental Listings Scraper automates the process of collecting rental property data from Zonaprop. It uses the `requests` library to fetch web pages, `BeautifulSoup` to parse HTML content, and regular expressions to clean and format data. The extracted data includes:

- **Prices** and **Expenses** of the rental properties.
- **Property Address** and **Description**.
- **Images** associated with the listings.
- **Features** such as services, rooms, and other characteristics.

The final output is saved in a CSV file, making it easy to analyze the collected data.

## Features

- **Web Scraping**: Automatically collects data from multiple pages of Zonaprop rental listings.
- **Data Cleaning**: Processes and cleans raw HTML to extract useful data.
- **CSV Export**: Saves the extracted data in a CSV file for easy access and analysis.
- **Error Handling**: Includes basic error handling to ensure the scraper runs smoothly even when encountering unexpected data.

## Prerequisites

- Python 3.x
- Required Python libraries: `requests`, `BeautifulSoup`, `urllib`, `re`, `csv`, `json`

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/zonaprop-rental-scraper.git
    cd zonaprop-rental-scraper
    ```

2. **Install the required libraries:**
    ```bash
    pip install requests beautifulsoup4
    ```

## Usage

1. **Run the scraper:**
    ```bash
    python main.py
    ```

    The scraper will start collecting rental data from Zonaprop and store it in `detalles_alquileres.csv`.

2. **Adjust the number of pages:**
    You can modify the number of pages to scrape by changing the argument in `ScrapeAlquileres(2)` within the `main.py` file.

## Example

The CSV file `detalles_alquileres.csv` will include columns such as:
- `precio`
- `expensas`
- `address`
- `description`
- `pictures`
- `servicios`
- `ambientes`
- `características`

