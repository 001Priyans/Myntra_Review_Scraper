# Myntra Review Scraper

[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-99.5%25-orange?style=flat&logo=jupyter)](https://jupyter.org/)
[![Python](https://img.shields.io/badge/Python-0.5%25-blue?style=flat&logo=python)](https://www.python.org/)

A web scraping tool designed to extract product reviews from Myntra, an e-commerce platform for fashion products. This tool helps in collecting customer feedback data for analysis and research purposes.

## 📋 Features

- Extract reviews from Myntra product pages
- Support for filtering reviews by rating
- Data export capabilities (CSV, JSON formats)
- Detailed data collection including:
  - Review text
  - Ratings
  - User information
  - Review dates
  - Helpful votes
  - Product information

## 🛠️ Installation

1. Clone this repository:
   ```
   git clone https://github.com/001Priyans/Myntra_Review_Scraper.git
   cd Myntra_Review_Scraper
   ```

2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## 📊 Usage

### Jupyter Notebook

1. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

2. Open the main scraper notebook (e.g., `myntra_review_scraper.ipynb`) and follow the instructions within.

### Python Script

If you prefer using the Python script directly:

```python
from myntra_scraper import MyntraReviewScraper

# Initialize the scraper
scraper = MyntraReviewScraper()

# Scrape reviews for a specific product
product_url = "https://www.myntra.com/product-page-url"
reviews = scraper.scrape_reviews(product_url)

# Export the data
scraper.export_to_csv(reviews, "product_reviews.csv")
```

## 📁 Project Structure

```
Myntra_Review_Scraper/
├── myntra_review_scraper.ipynb   # Main Jupyter notebook
├── scraper/
│   ├── __init__.py
│   └── myntra_scraper.py         # Core scraper functionality
├── examples/
│   └── example_usage.ipynb       # Example usage notebooks
├── data/
│   └── sample_data.csv           # Sample scraped data
├── requirements.txt              # Project dependencies
└── README.md                     # Project documentation
```

