# Café Branches Analytics Dashboard

A Power BI learning project focused on comparing sales performance across two café branches using clean data modeling, time intelligence, and interactive analytics.

---

## Project Goal
To design an analytical dashboard that enables:
- Comparison of sales across multiple branches
- Analysis of product and payment behavior
- Time-based performance tracking and basic revenue simulation

This project emphasizes **how the problem is approached**, not just the final visuals.

---

## Dataset Overview
- Two independent café sales streams
- Different payment structures across branches
- Transaction-level sales data with date, time, product, and payment attributes

---

## Analytical Approach
- Unified multiple data sources into a single fact table
- Built a **star schema** with dedicated dimension tables
- Created a custom Date table to support time intelligence
- Derived daypart categories from transaction time

---

## Key Concepts Demonstrated
- Data cleaning and shaping using Power Query
- Star schema data modeling
- DAX measures for:
  - MTD, YTD, YoY
  - Rolling period analysis
- Field parameters for dynamic metric and dimension switching
- What-if parameter for revenue simulation
- Bookmarks and synced slicers for interactive analysis

---

## Outcome
The dashboard enables structured analysis of:
- Sales trends over time
- Product-level performance
- Payment behavior differences across branches
- Simulated impact of price changes

---

## Tools Used
- Power BI Desktop
- Power Query
- DAX

---

## Note:
This project was built as a **learning and portfolio exercise** to demonstrate applied Power BI and BI modeling skills and is not an enterprise level project
