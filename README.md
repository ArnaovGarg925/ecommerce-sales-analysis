# Project 01 — E-Commerce Sales Analysis
**Pluto Academy Data Analytics Internship**

## Overview
Analysis of 12 months of e-commerce sales data (Olist Brazilian E-Commerce Dataset, Kaggle)
to identify revenue trends, top-performing categories and regions, and customer satisfaction
patterns — with a management dashboard and business insights report.

## Files in this repo
| File | Description |
|---|---|
| `Project1_Ecommerce_Sales_Analysis.ipynb` | Main notebook — data cleaning, 5 analysis questions, 6 charts, dashboard |
| `INSIGHTS_REPORT.md` | 5-point business insights report |
| `charts/` | All exported chart images (PNG), including the dashboard |
| `data/` | Source CSV files (Olist dataset subset used) |

## Tools used
Python · Pandas · Matplotlib · Seaborn (run in Google Colab)

## How to reproduce
1. Open `Project1_Ecommerce_Sales_Analysis.ipynb` in Google Colab or Jupyter.
2. Make sure the `data/` folder (with the Olist CSVs) is in the same directory, or update the
   `DATA` path in the first code cell.
3. Run all cells top to bottom.

## Key results
- **Total revenue analysed:** R$ 15,419,774 across 96,478 delivered orders
- **Top category by revenue:** Health & Beauty
- **Peak sales month:** November 2017 (Black Friday period)
- **Top-performing state:** São Paulo (SP)
- **Average order value:** R$ 159.83
- **Average review score:** 4.09 / 5 (57.8% five-star, 11.5% one-star)

See `INSIGHTS_REPORT.md` for the full write-up and recommendations.

## Data cleaning notes
- Only orders with status `delivered` are used for revenue analysis (cancelled/unavailable
  orders never generated real revenue).
- Missing product categories filled as `unknown` rather than dropped, to avoid losing revenue data.
- Duplicate rows checked and removed across all source tables.
- Category names translated from Portuguese to English for readability.
- Full step-by-step log is in the notebook's Data Cleaning section.
