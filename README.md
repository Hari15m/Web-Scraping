# Web-Scrapping: Python Projects for Data Extraction & Analysis

This repository contains Python scripts demonstrating end-to-end data pipelines: from scraping static and dynamic web content to cleaning, processing, and visualizing the final dataset.

## Repository Structure

| File/Directory | Description | Key Technologies |
| :--- | :--- | :--- |
| `beautifulsoup.py` | Scrapes data from static websites (e.g., `books.toscrape.com`). | Requests, Beautiful Soup |
| `selenium.py` | Scrapes data from dynamic, JavaScript-heavy websites (e.g., Amazon, requiring browser automation). | Selenium, Webdriver Manager |
| `visualisation.py` | Cleans scraped data and generates insightful charts (e.g., salary distribution). | Pandas, Matplotlib |
| `README.md` | **(This file)** Project overview and setup instructions. | Markdown |

-----

## 1\. Setup and Installation

### A. Clone the Repository

```bash
git clone https://github.com/YourUsername/Web-Scrapping.git
cd Web-Scrapping
```

### B. Create and Activate Virtual Environment

It is highly recommended to use a virtual environment to manage dependencies.

```bash
# Create the environment
python -m venv venv

# Activate the environment (Windows PowerShell)
.\venv\Scripts\Activate.ps1

# Activate the environment (macOS/Linux Bash)
source venv/bin/activate
```

### C. Install Dependencies

Install all necessary libraries, including those for scraping and visualization:

```bash
pip install requests beautifulsoup4 selenium pandas matplotlib webdriver-manager
```

-----

## 2\. Project Breakdown

### Project 1: Static Scraping (`beautifulsoup.py`)

This script demonstrates basic, fast, and polite web scraping of static HTML content using standard HTTP requests.

  * **Target:** Websites where content is fully loaded in the initial HTML response.
  * **Method:** Uses the `requests` library to fetch the HTML and **Beautiful Soup** to parse and extract data based on CSS selectors.
  * **Key Skills:** HTTP requests, HTML parsing, CSS selectors, error handling.

### Project 2: Dynamic Scraping (`selenium.py`)

This script handles modern websites that render content using JavaScript (e.g., Infinite scrolling, login forms).

  * **Target:** Websites like Amazon or complex e-commerce sites.
  * **Method:** **Selenium** automates a real browser (Chrome) to navigate, scroll, click buttons, and wait for elements to load before extracting data.
  * **Key Skills:** Browser automation, explicit waits (`WebDriverWait`), managing browser drivers (`webdriver-manager`), handling dynamic content.

### Project 3: Data Analysis & Visualization (`visualisation.py`)

This script takes the raw data collected from scraping and prepares it for analysis.

  * **Method:** Uses **Pandas** for cleaning (e.g., converting currency to float, standardizing categories) and **Matplotlib** for creating various charts.
  * **Outputs:** Generates charts that show key insights, such as salary distribution histograms and average salaries by experience level.
  * **Key Skills:** Data cleaning (Pandas), Data aggregation (`.groupby()`), Data visualization (`.plot()`, `matplotlib.pyplot`).

-----

## 3\. Usage

To run the full suite of scripts, execute them sequentially from your activated environment:

```bash
(venv) $ python beautifulsoup.py
(venv) $ python selenium.py
(venv) $ python visualisation.py
```

-----

*Created by [Hari15m]*
