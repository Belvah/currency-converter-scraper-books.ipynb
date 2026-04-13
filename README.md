# Web Scraping & Currency Converter

A Python project that scrapes book prices from books.toscrape.com and converts them into different currencies using a live exchange rate API.

## Project Overview

This project demonstrates:
- Web scraping with BeautifulSoup
- API integration for live currency conversion (frankfurter.app)
- Data cleaning with regex
- Data visualization with matplotlib
- Saving results to CSV and JSON

## Notebooks

| Notebook | Description |
|----------|-------------|
| `currency_converter_scraper_books.ipynb` | Scrapes book prices from books.toscrape.com and converts GBP to KES/USD/EUR |
| `scraping.ipynb` | Basic web scraping with pagination from books.toscrape.com |
| `apis.ipynb` | API usage examples (GET, POST, PUT, DELETE), regex, XML parsing, and OOP |
| `web_scraping.ipynb` | Web scraping fundamentals |

## Setup

1. Create and activate the virtual environment:
   ```bash
   python3 -m venv myenvt2
   source myenvt2/bin/activate
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run any notebook in VS Code with the `myenvt2` kernel selected.

## Tools & Technologies

- Python 3.13
- Jupyter Notebook
- VS Code
- Git & GitHub
- Frankfurter API (live exchange rates, no API key required)

## Libraries Used

- `requests` — HTTP requests for scraping and API calls
- `beautifulsoup4` — HTML parsing and data extraction
- `pandas` — Data manipulation and tabular display
- `matplotlib` — Data visualization (bar charts)
- `numpy` — Numerical operations for chart layout
- `re` — Regex for price data cleaning
- `json` — JSON data export
- `datetime` — Timestamping conversions
- `openpyxl` — Excel file support
- `lxml` — XML parsing

## Currency API

Uses the free [Frankfurter API](https://api.frankfurter.app/) for live exchange rates. No API key required.

### Supported Currencies

- GBP (British Pound)
- KES (Kenyan Shilling)
- USD (US Dollar)
- EUR (Euro)

## Output Files

- `books_converted.csv` / `books_converted.json` — Converted book prices

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/api_test.git
   cd api_test
   ```

2. Create a virtual environment:
   ```bash
   python3 -m venv myenvt2
   source myenvt2/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Testing

1. Open `currency_converter_scraper_books.ipynb` in VS Code.
2. Select the `myenvt2` kernel (top-right of notebook).
3. Run the cell and press **Enter** twice to use the default currencies (GBP → KES).
4. Verify that:
   - 10 books are scraped successfully
   - Exchange rate is fetched from the API
   - A table with original and converted prices is displayed
   - `books_converted.csv` and `books_converted.json` are created
   - A bar chart comparing original vs converted prices is shown

## Contributions

Ways to contribute:
- Add more currencies to the `supported_currencies` dictionary
- Scrape more pages (add pagination to get all 1000 books instead of 10)
- Add more e-commerce sites (e.g., Amazon, Jumia)
- Use a different exchange rate API as a backup
- Save data in different files like Excel, Text etc in addition to CSV/JSON)
- Improve the chart (add more visualization types like pie charts)
- Add unit tests

How to contribute:
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

## Contact

Belvah Shanyisa

GitHub: [Belvah](https://github.com/Belvah)