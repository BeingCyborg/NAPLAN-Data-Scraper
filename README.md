# NAPLAN Data Scraper

Scrapes Victorian school NAPLAN test results from myschool.edu.au. Collects scores across five domains (Reading, Writing, Spelling, Grammar, Numeracy) for year levels 3, 5, 7, and 9. Outputs structured CSV data for analysis.

## Technologies

- Python 3.8+
- Selenium (browser automation)
- Pandas (data processing)
- BeautifulSoup (HTML parsing)
- Jupyter Notebook

## Setup

Requires Python 3.8+ and Chrome browser.

```bash
pip install -r requirements.txt
jupyter notebook naplan_scraper.ipynb
```

## Configuration

Edit these variables in the notebook:

- `YEARS_TO_SCRAPE` - years to pull data for (default: [2023, 2024])
- `BETWEEN_REQUESTS_DELAY` - delay between requests in seconds (default: 2)
- `PAGE_LOAD_TIMEOUT` - page load timeout in seconds (default: 30)
- `max_pages` - number of school listing pages to scrape (3 for testing, 140 for all schools)
