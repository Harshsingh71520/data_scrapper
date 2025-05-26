# 📚 Book Scraper Project

This project demonstrates the usage of **BeautifulSoup** and **Pandas** in a simple web scraping application. The goal is to extract book data from a static HTML file (simulating a book store webpage), process it, and store the extracted data in a structured CSV file.

## 🚀 Features

- Parses a local HTML file using `BeautifulSoup`
- Extracts:
  - Book Title
  - Price (in £)
  - Rating (e.g., One, Two, Five)
- Uses `Pandas` to:
  - Organize the data into a DataFrame
  - Save the data into a CSV file for further analysis

## 🧰 Technologies Used

- Python
- BeautifulSoup (for HTML parsing)
- Pandas (for data manipulation and CSV export)

## 📁 File Structure

Scrapping/
├── page1.html # Sample HTML file to scrape
├── Booksdata.csv # Output CSV with scraped book data
├── script.py # Python script with scraping logic
└── README.md # Project description and usage


## 📝 How It Works

1. Load a local HTML file (`page1.html`) representing a page with books.
2. Use **BeautifulSoup** to extract:
   - Title from `<h3><a title="...">`
   - Price from `<p class="price_color">`, cleaned to remove '£'
   - Rating from `<p class="star-rating X">`, where `X` is the rating
3. Store the extracted data in a list.
4. Convert the list into a DataFrame using **Pandas**.
5. Save the DataFrame as `Booksdata.csv`.

## 📦 Output Example

| Book title             | Price | Rating |
|------------------------|-------|--------|
| It's Only the Himalayas| 45.17 | Two    |
| A Light in the Attic   | 51.77 | Three  |

## ✅ Requirements

- Python 3.x
- `beautifulsoup4`
- `pandas`

Install dependencies with:

```bash
pip install beautifulsoup4 pandas
