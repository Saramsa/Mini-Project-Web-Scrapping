GoodRx Drug Pricing – From Scraper to Insight
📄 Project Description
This project was developed for the DCS 625 – Text Mining and Web Scraping course at Carolina University (Summer 2025).
The main goal was to create a complete data pipeline to extract, clean, analyze, and interpret prescription drug prices from GoodRx.com.

Using Selenium-based scraping, the project collects real-time drug pricing from multiple U.S. cities (via ZIP codes), then applies cleaning and transformation steps to prepare the data for analysis.

Two primary analysis phases were conducted:

Exploratory Data Analysis (EDA) – uncover pricing trends, city-level differences, and the impact of special offers.

Natural Language Processing (NLP) – identify patterns in pharmacy and drug names, coupon usage, and promotional trends.

The outcome is a conceptual Drug Price Comparison Engine, demonstrating how data science can improve healthcare price transparency.

⚙️ Setup Instructions
1. Clone or download the repository
If using GitHub:

bash
Copy
Edit
git clone <repository_url>
cd <repository_folder>
If using a ZIP, extract it and open the folder.

2. Create and activate a virtual environment
bash
Copy
Edit
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Download NLTK resources (first-time only)
In Python:

python
Copy
Edit
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('averaged_perceptron_tagger')
5. Run the notebooks in order
Selenium_Web_Scraper.ipynb – Scrapes raw drug pricing data from GoodRx.

data_cleaning_goodrx.ipynb – Cleans and formats the scraped data.

exploratory_analysis_goodrx.ipynb – Performs EDA and visualization.

Hypothesis_nlp_analysis.ipynb – Runs NLP hypothesis testing and visualizations.

📦 Dependencies
Core Libraries

pandas

numpy

matplotlib

plotly

nltk

wordcloud

Web Scraping

selenium

undetected-chromedriver

Other Utilities

string

re

time

random

traceback

urllib

📂 Repository Structure
kotlin
Copy
Edit
.
├── data/
│   ├── raw/
│   │   └── scraped_goodrx_data.csv
│   └── processed/
│       └── goodrx_cleaned_data.csv
├── notebooks/
│   ├── Selenium_Web_Scraper.ipynb
│   ├── data_cleaning_goodrx.ipynb
│   ├── exploratory_analysis_goodrx.ipynb
│   └── Hypothesis_nlp_analysis.ipynb
├── requirements.txt
└── README.md
▶️ How to Run
Open each notebook in Jupyter or VS Code and execute cells sequentially.

Ensure Chrome browser is installed for Selenium.

The scraper will save results into scraped_goodrx_data.csv, which is then cleaned and analyzed.

📊 Outputs
Cleaned Data: goodrx_cleaned_data.csv

EDA Visualizations: price distributions, averages, offer breakdowns, online vs in-store comparisons, coupon effectiveness.

NLP Visualizations: POS tag frequencies, common bigrams, offer distributions by geography and channel.

✨ Key Insights
From the final analysis:

Pricing Variability – Prices differ significantly across cities and pharmacies.

Online Advantage – Online pharmacies tend to offer more consistent and lower pricing.

Special Offer Concentration – Promotions are most common in large urban centers.

Branding Patterns – Pharmacy names emphasize convenience, specialization, and online accessibility.

📌 License
This project is for educational purposes under the DCS 625 course requirements.
