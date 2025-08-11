# Mini-Project – Web Scrapping (GoodRx)

## 📄 Project Overview
This project automates extraction of prescription drug prices from **GoodRx.com** using Selenium, cleans the data with Python, and applies **EDA** and **NLP** to reveal pricing trends, special-offer patterns, and branding insights across cities—forming a conceptual **Drug Price Comparison Engine**.

---

## 🔗 Repository
**GitHub:** https://github.com/Saramsa/Mini-Project-Web-Scrapping  
Clone:
```bash
git clone https://github.com/Saramsa/Mini-Project-Web-Scrapping.git
cd Mini-Project-Web-Scrapping
```

---

## ⚙️ Setup

### 1) Create a virtual environment
```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

### 2) Install dependencies
```bash
pip install -r requirements.txt
```

### 3) One-time NLTK downloads
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('averaged_perceptron_tagger')
```

---

## ▶️ How to Run (Notebook order)
1. **`Selenium_Web_Scraper.ipynb`** – Scrapes GoodRx prices → outputs `scraped_goodrx_data.csv`
2. **`data_cleaning_goodrx.ipynb`** – Cleans & enriches → outputs `goodrx_cleaned_data.csv`
3. **`exploratory_analysis_goodrx.ipynb`** – EDA visualizations & summaries
4. **`Hypothesis_nlp_analysis.ipynb`** – NLP hypotheses (POS, bigrams, offers by city/online)

> Ensure Google Chrome is installed for Selenium (uses `undetected-chromedriver`).

---

## 📦 Dependencies
```
pandas
numpy
matplotlib
plotly
nltk
wordcloud
selenium
undetected-chromedriver
```
Install via:
```bash
pip install -r requirements.txt
```

---

## 📂 Suggested Structure
(Your repo may already match this.)
```
.
├─ scraped_goodrx_data.csv           # Raw scraped data
├─ goodrx_cleaned_data.csv           # Cleaned dataset
├─ Selenium_Web_Scraper.ipynb
├─ data_cleaning_goodrx.ipynb
├─ exploratory_analysis_goodrx.ipynb
├─ Hypothesis_nlp_analysis.ipynb
├─ requirements.txt
└─ README.md
```

---

## 📊 Outputs & Insights
- **Cleaned data** ready for analysis
- **EDA**: price distributions, averages, outliers, special-offer breakdowns, online vs in-store comparisons
- **NLP**: POS tag frequencies, common bigrams, city-wise and channel-wise (online/offline) offer patterns

---

## 📌 Notes
- Be polite with delays between requests (`time.sleep`) to avoid stressing target servers.
- Paths are relative; keep files in repo root or adjust paths in notebooks accordingly.
