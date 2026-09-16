# 🕸️ Wikipedia Web Scraper — Largest US Companies by Revenue

A small demo project that scrapes Wikipedia's [List of largest companies in the United States by revenue](https://en.wikipedia.org/wiki/List_of_largest_companies_in_the_United_States_by_revenue) 📊 and loads the data into a pandas DataFrame for further analysis.

## ✨ What it does

- 🌐 Sends a request to the Wikipedia page with a proper `User-Agent` header (required — Wikipedia blocks unidentified bots)
- 🍜 Parses the HTML with BeautifulSoup
- 🔍 Locates the "largest public companies" table
- 🧹 Extracts column headers and row data
- 🐼 Builds a clean pandas DataFrame with columns: Rank, Name, Industry, Revenue (USD millions), Revenue growth, Employees, Headquarters

## 🛠️ Tech stack

- 🐍 Python
- 📡 `requests` — fetching the page
- 🍲 `beautifulsoup4` — parsing HTML
- 🐼 `pandas` — structuring the scraped data

## 🚀 Setup

1. Clone this repo:
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open and run the notebook:
   ```bash
   jupyter notebook
   ```

## 📝 Notes

- ⚠️ Wikipedia requires a valid `User-Agent` header on requests; without one, it returns a placeholder page instead of the real content.
- 🙏 This project is for learning/demo purposes — scraping etiquette (rate limiting, identifying your bot) should always be followed when working with live websites.

## 📈 Example output

| Rank | Name | Industry | Revenue (USD millions) | Revenue growth | Employees | Headquarters |
|------|------|----------|------------------------|-----------------|-----------|--------------|
| 1 | Walmart | Retail | 680,985 | ▲ 5.1% | 2,100,000 | Bentonville, Arkansas |
| 2 | Amazon | Retail and cloud computing | 637,959 | ▲ 11.0% | 1,556,000 | Seattle, Washington |

---

⭐ If you found this useful, feel free to star the repo!
