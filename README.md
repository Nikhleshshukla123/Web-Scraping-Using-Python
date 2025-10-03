# Amazon Product Scraper

## Project Overview
This project is a Python-based web scraper that collects product information from Amazon search results. Using **Requests** and **BeautifulSoup**, it extracts details such as product title, price, rating, number of reviews, and availability status, and saves the data into a CSV file for further analysis.

---

## Features
- Scrapes multiple pages of Amazon search results.  
- Extracts product information:
  - Product Title  
  - Price  
  - Rating  
  - Number of Reviews  
  - Availability  
- Saves the collected data to a CSV file.  
- Includes **error handling** and polite delays to avoid blocking by Amazon.  

---

## Technologies Used
- Python 3.x  
- Libraries:
  - `requests` – for making HTTP requests  
  - `BeautifulSoup` – for parsing HTML  
  - `pandas` – for data storage and manipulation  
  - `numpy` – for handling missing values  
  - `time` and `random` – for delays between requests  

---

## Project Structure
amazon_scraper/
│
├── amazon_scraper.ipynb # Jupyter notebook with the full scraping workflow
├── amazon_data.csv # CSV output file with scraped data
├── README.md # Project documentation
└── requirements.txt # Required Python libraries


---

## Usage
1. Clone the repository or oprn the notebook in kaggle/local jupyter.
2. Install the required libraries

```bash
pip install -r requirements.txt

3. Open the notebook and run the cells in order.
4. Scraped product data will be saved as:

/kaggle/working/amazon_data.csv  (Kaggle)
or amazon_data.csv (Local)

5. You can modify the search term and number of pages to scrape:
BASE_URL = "https://www.amazon.com/s?k=playstation+5&page="
TOTAL_PAGES = 5

6. Output Example
<img width="989" height="371" alt="image" src="https://github.com/user-attachments/assets/3dd602af-f9e0-4717-985a-286c24aba31e" />
