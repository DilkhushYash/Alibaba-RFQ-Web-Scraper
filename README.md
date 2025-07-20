# 🕸️ Alibaba RFQ Web Scraper

This project is a Python-based web scraping tool that extracts **RFQ (Request for Quotation)** listings from Alibaba's sourcing platform:

🔗 [Target URL](https://sourcing.alibaba.com/rfq/rfq_search_list.htm?spm=a2700.8073608.1998677541.1.82be65aaoUUItC&country=AE&recently=Y&tracelog=newest)

The scraper automatically navigates through **all pages**, extracts RFQ details, and saves them into a structured CSV file for analysis or business use.

## 📌 Project Overview

- Scrapes **all RFQ listings** from the specified country (UAE)
- Extracts essential information such as:
  - **Title of the RFQ**
  - **Product Category**
  - **Buyer Country**
  - **Submission Date**
  - **RFQ Details**
- Cleans and compiles the data into `Final.csv`

## 🛠️ Technologies Used

- Python 3
- `requests`
- `BeautifulSoup` (bs4)
- `pandas`
- `time`
- Jupyter Notebook

## 📂 Project Structure

| File Name            | Description                                                   |
|----------------------|---------------------------------------------------------------|
| `Intern scrape.ipynb`| Jupyter Notebook with full scraping, pagination, and CSV logic|
| `Final.csv`          | Final output with all scraped RFQ entries from Alibaba        |

## 🚀 How It Works

1. Sends HTTP requests to Alibaba's paginated RFQ listing URLs.
2. Parses the HTML response using BeautifulSoup.
3. Extracts all relevant RFQ data.
4. Cleans and organizes the data.
5. Appends to a pandas DataFrame and exports to `Final.csv`.

## 📊 Sample Output (`Final.csv`)

| Title                      | Category         | Country | Date       | Description                          |
|----------------------------|------------------|---------|------------|--------------------------------------|
| Buy Face Masks             | Health & Medical | UAE     | 2025-07-19 | Need 100K pcs 3-layer face masks     |
| Purchase LED Light Strips  | Lights & Lighting| UAE     | 2025-07-18 | Looking for waterproof LED strip     |

> 🔍 Full dataset is available in the included `Final.csv`

## 💡 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/alibaba-rfq-scraper.git
   cd alibaba-rfq-scraper
   ```
2.Install the dependencies:
```bash
pip install -r requirements.txt
```
3.Open and run the scraper:
```bash
jupyter notebook "Intern scrape.ipynb"
```
## 🧠 Future Enhancements
  - Add filters for RFQ keywords, quantity, or specific dates

  - Export results to Excel or JSON

  - Add GUI using Streamlit or Tkinter

  - Integrate scheduling for automated scraping

Yash Dilkhush

B.Tech CSE @ SCET, Surat

Frontend Engineer • Data Analyst • Web Scraping Enthusiast

📧 yashdilkhush96@gmail.com
