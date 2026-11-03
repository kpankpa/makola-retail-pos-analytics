# Makola Market Retail & POS Analytics Case Study

## Project Overview
This project analyzes over 120,000 retail transactions from open-air market trading to uncover key business drivers around sales margins, customer retention, and inventory risks. 

The goal of this analysis is to evaluate the commercial case for moving traditional micro-merchants from paper ledgers to digital tablet POS systems (like Caris Retail Cloud). It also builds alternative credit and inventory risk metrics that banks and suppliers can use to evaluate unbanked traders.

---

## Business Problem & Objectives
In high-density traditional markets like Makola Market in Accra, informal retailers often struggle with:
* Unclear profit margins due to mixed product pricing and manual record-keeping.
* High stockout rates during peak market hours.
* Difficulty securing working capital loans because they lack formal credit histories.

This notebook processes transaction logs to answer three core operational questions:
1. Which product categories drive raw revenue versus actual net profitability?
2. How do customer purchasing patterns break down by lifetime value and retention?
3. How quickly do different store formats convert stock into cash, and which categories carry the highest stockout risk?

---

## What's Inside the Analysis
The main Jupyter notebook (`makola-market-retail-analytics.ipynb`) is structured into six sequential steps:

1. **Data Cleaning & Hygiene:** Standardizing schema formats, checking missing values, and preparing transactional variables.
2. **Sales & Margin Performance:** Comparing gross margins and sales revenue across store formats and product lines.
3. **Customer Lifetime Value (CLV) & Segmentation:** Grouping shoppers by average spend, retention rate, and engagement level.
4. **Product Affinity & Correlation:** Analyzing feature relationships (revenue, discounts, units sold, stockout rates) using matrix correlations.
5. **Item Co-Occurrence:** Building a pure-pandas basket matrix to see which product categories are routinely purchased together.
6. **Vendor Liquidity & Stockout Risk Modeling:** Estimating cash conversion velocity and scoring categories most vulnerable to inventory depletion.

---

## Tech Stack & Tools
* **Language:** Python 3
* **Libraries:** Pandas, Matplotlib

---

## Repository Structure
```
├── notebooks/
│   └── makola-market-retail-analytics.ipynb   # Main Jupyter Notebook
├── data/
│   └── supermarket_large_dataset.csv          # Transaction dataset
├── README.md                                  # Executive summary and docs
└── requirements.txt                           # Python dependencies
```

---

## Quick Start (How to Run)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/makola-market-retail-analytics.git
   cd makola-market-retail-analytics
   ```

2. **Install required packages:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Open the notebook:**
   ```bash
   jupyter lab
   ```