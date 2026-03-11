# Café Branches Analytics Dashboard

A Power BI project focused on comparing sales performance across two café branches using Python-based data preparation, clean data modeling, time intelligence, and interactive analytics.
<img width="1253" height="702" alt="cafe_pg1" src="https://github.com/user-attachments/assets/6f197a0d-1277-457a-bc23-698327004cbc" />

---

## Project Goal

To design an analytical dashboard that enables:
- Comparison of sales across multiple branches
- Analysis of product and payment behavior
- Time-based performance tracking

This project emphasizes **how the problem is approached**, not just the final visuals.

---

## Data Pipeline

```
Raw CSVs (index_1.csv, index_2.csv)
        ↓
Python (pandas) — cleaning, transformation & merging
        ↓
Merged dataset → Power BI
```

Data from two sources was cleaned and unified into a single fact table using pandas. See [`cafe_transformed.ipynb`](cafe_transformed.ipynb) for the full transformation steps.

---

## Dataset Overview

- Two independent café sales streams
- Different payment structures across branches
- Transaction-level sales data with date, time, product, and payment attributes

---

## Dashboard Pages

**Overview** — High-level sales performance across branches. Tracks Total Revenue, MTD Sales, YTD Sales, and YoY growth with branch and payment type breakdowns. Bookmark-driven buttons switch between Total, MTD, and YTD views.

**Product Focus** — Product-level revenue and MTD sales by coffee name, with YoY % comparison across products.

**Customer Spending Behavior** — Transaction volume by customer card and revenue split by time period (daypart), with payment type and branch filters.

---

## Analytical Approach

- Unified multiple data sources into a single fact table
- Built a **star schema** with dedicated dimension tables (Product, Payment, Customer, Stream, Time, Date)
- Created a custom Date table to support time intelligence
- Derived daypart categories from transaction time

---

## Key Concepts Demonstrated

- End-to-end data pipeline: Python → Power BI
- Data cleaning and transformation using pandas
- Star schema data modeling
- DAX measures: Total Revenue, Total Sales, MTD Sales, YTD Sales, YoY Sales %
- Bookmarks for toggling between MTD, YTD, and Total views
- Synced slicers across pages (Date, Branch, Payment Type, Time Period)

---

## Tools Used

- Python (pandas)
- Power BI Desktop
- Power Query
- DAX

---

## Files

| File | Description |
|---|---|
| `cafe_transformed.ipynb` | Data cleaning and transformation (Python/pandas) |
| `Cafe Branches Data/` | Raw source CSVs |
| `Cafe_Dashboard_v1-basic.pbix` | Initial dashboard version |
| `Cafe_Dashboard_v2.pbix` | Final dashboard version |

---

## Note

This project was built as a **learning and portfolio exercise** to demonstrate applied Python, Power BI, and BI modeling skills, and is not an enterprise-level project.
