# E-Commerce Analytics Dashboard — Olist Brazil

An end-to-end analysis of the Olist Brazilian e-commerce dataset, covering data cleaning, exploratory analysis in Python, and an interactive Power BI dashboard.

## Project Overview

This project analyzes ~99K orders from Olist, a Brazilian e-commerce marketplace, to uncover revenue trends, top-performing product categories, geographic sales concentration, and customer satisfaction patterns between 2016 and 2018.

## Dataset

Source: [Olist Brazilian E-Commerce Public Dataset (Kaggle)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The raw dataset consists of 8 CSV files (orders, order items, customers, products, sellers, payments, reviews, and category translations), merged into a single cleaned master table for analysis.

> **Note:** Due to file size, the raw CSVs are not included in this repo. Download the dataset from Kaggle and place the CSVs in a local data/folder before running the notebook.

## Tools Used

- **Python** (Pandas) — data cleaning, merging, and aggregation
- **Plotly** — exploratory visualizations
- **Power BI** — interactive dashboard
- **Jupyter Notebook** — analysis workflow

## Key Findings

- **Average Order Value (AOV):** R$ 137.75
- **Total Revenue:** R$ 13.59M across 99K orders
- **Top product categories by revenue:** `health_beauty` (R$ 1.26M) and `watches_gifts` (R$ 1.21M) led, followed by `bed_bath_table`, `sports_leisure`, and `computers_accessories`
- **Geographic concentration:** São Paulo (SP) generated R$ 5.20M in revenue — more than double Rio de Janeiro (R$ 1.82M), the next-highest state
- **Seasonality:** Revenue grew steadily from late 2016 through 2018, with a sharp spike in November 2017 (R$ 1.01M), consistent with Black Friday
- **Customer satisfaction:** Average review score of 4.03 out of 5

## Files in This Repo

| File | Description |
|---|---|
| `Ecommerce_Analytics.ipynb` | Python notebook — data cleaning, merging, and exploratory analysis |
| `Ecommerce_Analytics_Dashboard.pbix` | Power BI dashboard file |
| `data/` | Folder for the Olist dataset CSVs (download separately from Kaggle) |

## Dashboard Preview

*(Add a screenshot of your Power BI dashboard here once finalized — drag the image into this README on GitHub, or use `![Dashboard](path/to/screenshot.png)`)*

## Limitations

- Revenue figures are based on item price only and exclude freight cost
- First (Sep 2016) and last (Sep 2018) months contain partial data and were excluded from trend analysis
- Dataset ends mid-2018, so no post-2018 trends can be inferred

## Next Steps

- Incorporate delivery time and freight cost to assess their effect on review scores
- Segment AOV and category preferences by state
- Explore repeat-customer behavior and retention patterns

## Author

Vandana Uppala
