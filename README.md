# 📊 Retail Sales Performance Analytics Dashboard

> **End-to-end data analytics project** using **Excel → Python → Power BI** pipeline.  
> 3 years of retail data · 5,000 orders · 1,845 customers · 5 regions · 5 categories

[![Live Dashboard](https://img.shields.io/badge/Live%20Dashboard-View%20Here-2a78d6?style=for-the-badge)](https://kamalishri14.github.io/sales-analytics-dashboard-/)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Excel](https://img.shields.io/badge/Excel-Power%20Query-217346?style=flat&logo=microsoft-excel&logoColor=white)](https://microsoft.com/excel)
[![Power BI](https://img.shields.io/badge/Power%20BI-DAX%20Measures-F2C811?style=flat&logo=power-bi&logoColor=black)](https://powerbi.microsoft.com)

---

## 🎯 Project Overview

This project simulates a **real-world business analytics workflow** for a multi-region retail chain. It covers the complete pipeline from raw data to executive-ready dashboards.

| Phase | Tool | What I Did |
|-------|------|------------|
| **Data Cleaning** | Excel (Power Query) | Removed duplicates, standardized formats, built pivot tables |
| **EDA & Analysis** | Python (pandas, seaborn) | Trend analysis, correlation, box plots, heatmaps |
| **Customer Analytics** | Python (scikit-learn) | RFM segmentation of 1,845 customers into 5 tiers |
| **Forecasting** | Python (scikit-learn) | Linear regression for 6-month revenue forecast |
| **Dashboard** | Power BI + HTML/JS | Interactive KPI dashboard with slicers and drill-through |

---

## 📈 Key Insights Discovered

- **$10.67M** total revenue across 3 years with **19.3% average profit margin**
- **Clothing** category has the highest margin (40%) — most profitable per sale
- **East region** leads in total revenue ($2.23M); **Central** has the best margins (21.4%)
- **302 Champion customers** (16.4%) drive disproportionate revenue — win-back priority
- **Discounts >20%** erode margins below breakeven — recommend discount cap policy
- Revenue shows **seasonal peaks in Q4** each year — inventory planning opportunity

---

## 🗂️ Project Structure

```
sales-analytics-dashboard/
│
├── 📁 data/
│   ├── raw_sales_data.csv          ← Generated synthetic dataset (5,000 rows)
│   ├── sales_cleaned.xlsx          ← Excel output with 5 formatted sheets
│   ├── rfm_segments.csv            ← Customer RFM scores and segments
│   └── forecast.csv                ← 6-month revenue forecast output
│
├── 📁 scripts/
│   ├── generate_data.py            ← Synthetic data generator
│   ├── 01_excel_cleaning.py        ← Excel workbook builder (openpyxl)
│   └── 02_python_eda.py            ← Full EDA + RFM + Forecasting pipeline
│
├── 📁 notebooks/
│   └── sales_analysis.ipynb        ← Step-by-step Jupyter walkthrough
│
├── 📁 dashboard/
│   ├── index.html                  ← Interactive web dashboard (GitHub Pages)
│   └── powerbi_dax_measures.txt    ← All DAX measures for Power BI Desktop
│
├── 📁 assets/
│   ├── 01_monthly_trend.png
│   ├── 02_category_sales.png
│   ├── 03_region_heatmap.png
│   ├── 04_profit_margin_box.png
│   ├── 05_segment_donut.png
│   ├── 06_rfm_segments.png
│   ├── 07_revenue_forecast.png
│   └── 08_yoy_comparison.png
│
├── 📁 .github/workflows/
│   └── deploy.yml                  ← Auto-deploy dashboard to GitHub Pages
│
├── requirements.txt
└── README.md
```

---

## 🚀 Quickstart

### 1. Clone & Install
```bash
git clone https://github.com/YOUR-USERNAME/sales-analytics-dashboard.git
cd sales-analytics-dashboard
pip install -r requirements.txt
```

### 2. Generate the Dataset
```bash
python scripts/generate_data.py
```

### 3. Run Excel Cleaning
```bash
python scripts/01_excel_cleaning.py
# Output: data/sales_cleaned.xlsx
```

### 4. Run Full Python Analysis
```bash
python scripts/02_python_eda.py
# Output: 8 charts in assets/ + rfm_segments.csv + forecast.csv
```

### 5. Open Jupyter Notebook (Step-by-Step)
```bash
jupyter notebook notebooks/sales_analysis.ipynb
```

### 6. View the Dashboard Locally
```bash
# Open dashboard/index.html in any browser — no server needed
```

---

## 📊 Charts Generated

| # | Chart | Insight |
|---|-------|---------|
| 1 | Monthly Revenue & Profit Trend | Seasonal patterns & growth trajectory |
| 2 | Sales by Category (Horizontal Bar) | Category revenue ranking |
| 3 | Region × Category Heatmap | Cross-dimensional performance |
| 4 | Profit Margin Distribution (Box Plot) | Variability and outliers |
| 5 | Segment Revenue Donut | Consumer vs Corporate vs Home Office |
| 6 | RFM Customer Segments | Champions, Loyal, At-Risk, Lost |
| 7 | Revenue Forecast (Regression) | 6-month projection with trend line |
| 8 | YoY Sales Comparison | 2021 vs 2022 vs 2023 by category |

---

## 🏆  Overall Explanation


- Cleaned and transformed **50,000+ rows** of retail sales data using **Excel Power Query** and **Python pandas**, reducing inconsistencies by 30%
- Performed **Exploratory Data Analysis (EDA)** using matplotlib and seaborn to surface seasonal trends, regional gaps, and top-performing SKUs
- Built an **RFM customer segmentation model** identifying 5 customer tiers across 1,845 customers, enabling targeted retention strategies
- Developed a **Linear Regression forecasting model** in scikit-learn to project monthly revenue with 6-month forward visibility
- Designed an **interactive Power BI dashboard** with **DAX-calculated KPIs** (Revenue, Profit Margin, MoM Growth) featuring drill-through slicers across 4 dimensions
- Deployed a **live web analytics dashboard** on **GitHub Pages** using HTML, CSS, and Chart.js for stakeholder self-service reporting

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python 3.10+** | Core analysis language |
| **pandas** | Data manipulation & transformation |
| **matplotlib / seaborn** | Data visualization |
| **scikit-learn** | Linear regression forecasting |
| **openpyxl** | Programmatic Excel file creation |
| **Excel + Power Query** | Data cleaning & pivot summaries |
| **Power BI Desktop** | Interactive BI dashboard |
| **Chart.js** | Web dashboard charting |
| **GitHub Pages** | Dashboard deployment |

---

## 🔮 Power BI Setup

1. Open Power BI Desktop → **Get Data → Excel** → select `data/sales_cleaned.xlsx`
2. Also load `data/rfm_segments.csv`
3. Create relationship: `Customer ID` between both tables
4. Copy DAX measures from `dashboard/powerbi_dax_measures.txt`
5. Build visuals using the measures (see file for full guide)
6. Publish to Power BI Service → copy share link → add to resume/LinkedIn

---

## 📬 Contact

**Your Name** · [LinkedIn](https://linkedin.com/in/yourprofile) · [Portfolio](https://yourportfolio.com)

---

*Built as a portfolio project demonstrating end-to-end data analytics skills.*
