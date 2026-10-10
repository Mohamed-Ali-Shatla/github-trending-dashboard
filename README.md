# GitHub Trending Dashboard

## Project Overview
A simple project that scrapes the trending repositories from GitHub, saves them to a CSV file, and shows them in an interactive Dash dashboard. Everything is in one notebook: `github_trending_dashboard.ipynb`.

## Data Source
- https://github.com/trending (daily, weekly and monthly)
- Scraped with **BeautifulSoup**
- Saved to `trending_repos.csv` (created when you run the notebook)

## Dashboard Features
- **Filter:** dropdown to choose the period (daily / weekly / monthly)
- **4 KPI cards:** number of repositories, total stars, total forks, top language
- **2 charts:** top 10 trending repositories (bar chart) and programming language distribution (pie chart)

## How to Run
1. Install Python and Jupyter:
   ```
   pip install notebook
   ```
2. Open the notebook:
   ```
   jupyter notebook github_trending_dashboard.ipynb
   ```
3. Run all the cells from top to bottom (Kernel > Restart & Run All).
   - The scraping cell downloads the data and creates `trending_repos.csv`.
   - The last cell starts the dashboard. If it doesn't appear inside the notebook, open http://127.0.0.1:8050 in your browser.
