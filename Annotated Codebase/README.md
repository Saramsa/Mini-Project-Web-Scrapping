# GoodRx Drug Pricing – From Scraper to Insight

## 📌 Project Description
This project focuses on extracting real-time prescription drug pricing data from **GoodRx** using Selenium WebDriver, cleaning and transforming the data with Python (Pandas, NumPy), and conducting exploratory data analysis (EDA) and NLP-based hypothesis testing. The goal is to identify price variations, special offers, and pharmacy-specific patterns across multiple cities in the US.

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/GoodRx-Drug-Pricing-Analysis.git
cd GoodRx-Drug-Pricing-Analysis
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Download NLTK Resources (First Run Only)
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('averaged_perceptron_tagger')
```

### 4️⃣ Run the Selenium Scraper
Update **`drug_urls`** and **`zip_codes`** in `Selenium_Web_Scraper.ipynb` if needed, then run the scraper to generate `scraped_goodrx_data.csv`.

### 5️⃣ Clean the Data
Run `data_cleaning_goodrx.ipynb` to produce `goodrx_cleaned_data.csv`.

### 6️⃣ Perform EDA & NLP Analysis
Run:
- `exploratory_analysis_goodrx.ipynb` → Data visualizations and statistical summaries.
- `Hypothesis_nlp_analysis.ipynb` → Hypothesis testing and text analysis.

---

## 📂 Repository Structure
```
.
├── Selenium_Web_Scraper.ipynb       # Web scraping with Selenium
├── data_cleaning_goodrx.ipynb       # Data cleaning and transformation
├── exploratory_analysis_goodrx.ipynb # EDA visualizations
├── Hypothesis_nlp_analysis.ipynb    # NLP hypothesis testing
├── scraped_goodrx_data.csv          # Raw scraped data
├── goodrx_cleaned_data.csv          # Cleaned dataset
├── requirements.txt                 # Python dependencies
└── README.md                        # Project documentation
```

---

## 🛠 Dependencies
Main libraries used:
- `selenium`
- `pandas`
- `numpy`
- `plotly`
- `matplotlib`
- `nltk`
- `wordcloud`

Install all dependencies:
```bash
pip install -r requirements.txt
```

---

## 📊 Key Features
- Automated web scraping of real-time GoodRx drug pricing
- Multi-location data collection via ZIP codes
- Data cleaning and transformation pipeline
- Exploratory data analysis with interactive visualizations
- NLP-based insights from pharmacy and drug names
- Hypothesis testing on pricing and offers

---

## 📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
