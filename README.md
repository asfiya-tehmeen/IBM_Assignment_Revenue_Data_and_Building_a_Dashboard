# 📊 Stock & Revenue Dashboard — Tesla & GameStop

> A data analytics project that extracts historical stock prices and quarterly revenue data for **Tesla (TSLA)** and **GameStop (GME)**, then visualizes them in a dual-panel dashboard built entirely in Python.

---

## 🗂 Project Overview

This project was completed as part of the **IBM Data Science Professional Certificate** on Coursera (Course: *Python Project for Data Science*). The goal is to simulate the workflow of a Junior Data Analyst — collecting, cleaning, and visualizing financial data to surface trends and insights for investors.

The notebook covers two parallel workflows:

| Task | Tesla (TSLA) | GameStop (GME) |
|---|---|---|
| Stock Data | `yfinance` API | `yfinance` API |
| Revenue Data | Web Scraping | Web Scraping |
| Dashboard | Matplotlib | Matplotlib |

---

## 🔧 Tech Stack

| Library | Purpose |
|---|---|
| `yfinance` | Pulling historical stock price data via Yahoo Finance |
| `requests` | HTTP requests to download revenue HTML pages |
| `BeautifulSoup` (`bs4`) | Parsing HTML and scraping revenue tables |
| `pandas` | Data manipulation and cleaning |
| `matplotlib` | Plotting the stock price and revenue dashboards |

---

## 📁 Project Structure

```
├── Revenue_Data_and_Building_a_Dashboard.ipynb   # Main Jupyter Notebook
└── README.md                                      # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.7+ and install the required libraries:

```bash
pip install yfinance bs4 requests pandas matplotlib
```

### Running the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/stock-revenue-dashboard.git
   cd stock-revenue-dashboard
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Revenue_Data_and_Building_a_Dashboard.ipynb
   ```

3. Run all cells from top to bottom (`Kernel → Restart & Run All`).

---

## 📌 Questions Solved

### Question 1 — Tesla Stock Data (yfinance)
Extracts the full historical stock price for Tesla using `yfinance`, resets the DataFrame index, and previews the first 5 rows.

### Question 2 — Tesla Revenue Data (Web Scraping)
Scrapes quarterly revenue figures for Tesla from an IBM-hosted HTML page using `requests` and `BeautifulSoup`. Cleans currency symbols and null values.

### Question 3 — GameStop Stock Data (yfinance)
Same approach as Q1, applied to GameStop (`GME` ticker).

### Question 4 — GameStop Revenue Data (Web Scraping)
Same scraping approach as Q2, applied to the GameStop revenue page.

### Question 5 — Tesla Dashboard
Plots Tesla's historical share price alongside its quarterly revenue using the `make_graph` function (data shown up to June 2021).

### Question 6 — GameStop Dashboard
Plots GameStop's historical share price alongside its quarterly revenue (data shown up to June 2021).

---

## 📈 Sample Output

The dashboard for each company renders two stacked panels:

- **Top panel** — Historical Share Price (USD)
- **Bottom panel** — Quarterly Revenue (USD Millions)

This layout makes it easy to visually compare how revenue performance correlates with stock price movements over time.

---

## 🧠 Key Concepts Demonstrated

- **Web scraping** with `requests` + `BeautifulSoup`
- **API-based data extraction** with `yfinance`
- **Data cleaning** — removing currency symbols, handling nulls, type casting
- **Data visualization** — multi-panel time series plots with `matplotlib`
- **Pandas** — DataFrame construction, filtering, concatenation

---

## 📜 License

This project is based on coursework from the [IBM Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science) on Coursera. Original lab authored by Joseph Santarcangelo & Azim Hirjani © IBM Corporation 2020.

---

## 🙋 Author

**Asfiya Tehmeen**  
[GitHub](https://github.com/asfiya-tehmeen) • [LinkedIn](https://www.linkedin.com/in/asfiya-tehmeen/)
