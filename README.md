# 🏦 Barclays Customer Churn Analysis

> **Power BI Data Analytics Project | Banking Domain**
>
> Analyst: **Rajeev Kumar** | Tool: Power BI

---

## 📌 Project Overview

This project analyzes **customer churn data for Barclays Bank** across three European countries — France, Germany, and Spain. The goal was to understand which customers are leaving, why they might be leaving, and what patterns exist in the data that can help with retention strategy.

| Detail | Information |
|--------|-------------|
| **Domain** | Banking — Customer Retention |
| **Total Customers** | 10,000 records |
| **Countries** | France · Germany · Spain |
| **Time Period** | January 2016 — December 2019 |
| **Overall Churn Rate** | 20.37% |

---

## 🛠️ Tools & Features Used

| Tool / Feature | Purpose |
|----------------|---------|
| **Power BI Desktop** | Building the full dashboard |
| **DAX (Data Analysis Expressions)** | Custom measures — Churn Rate, MTD, QTD, YTD, SPLY |
| **Power Query** | Data cleaning and transformation |
| **Dynamic DAX Time Series** | Compare performance across time periods |
| **Slicers & Filters** | Filter by Active Category, Gender, Customer Category |
| **Bookmarks & Navigation Buttons** | Smooth switching between report pages |

---

## 📁 Project Structure

```
Barclays-Customer-Churn-Analysis/
│
├── 📂 branding/                                 # Branding assets
├── 📂 Dataset/                                  # Raw dataset files
│
├── 📂 POWer Bi/
│   ├── 📊 Barclays_Cuustomer_Churn_Analysis.pbix   # Main Power BI file
│   ├── 📄 Barclays_Cuustomer_Churn_Analysis.pdf    # PDF export of the report
│   └── 📂 Screenshots/
│       ├── dashboard_page_1.png                 # Home Page
│       ├── dashboard_page_2.png                 # Main Dashboard
│       ├── dashboard_page_3.png                 # Customer Wise Analysis
│       ├── dashboard_page_4.png                 # Time Series Analysis
│       └── dashboard_page_5.png                 # Insights & Outcomes
│
├── 📄 Bank_Churn_PTP.docx                       # Project planning document
└── 📄 README.md
```

---

## 🖥️ Dashboard Pages

### Page 1 — Home
![Home]([POWer%20Bi/Screenshots/dashboard_page_1.png](https://github.com/reactwithrajeev/Barclays-Customer-Churn-Analysis/blob/main/POwer%20Bi/Screenshots/dashboard_page_1.png))

### Page 2 — Main Dashboard
![Dashboard](POWer%20Bi/Screenshots/dashboard_page_2.png)

### Page 3 — Customer Wise Analysis
![Customer Wise Analysis](POWer%20Bi/Screenshots/dashboard_page_3.png)

### Page 4 — Time Series Analysis
![Time Series Analysis](POWer%20Bi/Screenshots/dashboard_page_4.png)

### Page 5 — Insights & Outcomes
![Insights](POWer%20Bi/Screenshots/dashboard_page_5.png)

---

## 📊 Dashboard KPIs

| KPI | Value |
|-----|-------|
| Total Customers | 10,000 |
| Churn Rate | 20.37% |
| Total Exited Customers | 2,000 |
| Total Active Members | 5,000 |
| Total Inactive Members | 5,000 |
| Total Retained Customers | 8,000 |

---

## 📈 DAX Measures Written

```
Churn Rate %        = DIVIDE([Total Exited Customers], [Total Customers], 0) * 100
Total MTD           = CALCULATE([Total Customers], DATESMTD('Date'[Date]))
Total QTD           = CALCULATE([Total Customers], DATESQTD('Date'[Date]))
Total YTD           = CALCULATE([Total Customers], DATESYTD('Date'[Date]))
SPLY                = CALCULATE([Total Customers], SAMEPERIODLASTYEAR('Date'[Date]))
Dynamic TimeSeries  = Switches between MTD, QTD, YTD, SPLY based on slicer selection
```

---

## 🔍 Page Wise Analysis

### Page 2 — Main Dashboard
- KPI cards for all 6 key metrics
- Monthly line chart — Total Customers vs Exited Customers across 12 months
- Bar chart — Active members by Gender and Customer Remarks
- Geography bar chart — France, Germany, Spain comparison
- Donut chart — Churn Rate % by Geography Location

### Page 3 — Customer Wise Analysis
- Matrix table — Monthly customer count by country (France, Germany, Spain)
- Horizontal bar chart — Active vs Inactive Members by Age Group
- Scatter plot — Avg Estimated Salary vs Age by Gender (Correlation + Animation toggle)

### Page 4 — Time Series Analysis
- Drill-down chart — Customers by Year → Quarter → Month → Day
- Line chart with forecast — Customers and Churn Rate by Year and Quarter
- Bar chart — Total Customers and Dynamic DAX TimeSeries by Year
- Toggle buttons — SPLY · Total MTD · Total QTD · Total YTD

### Page 5 — Insights & Outcomes
- Auto-generated Power BI smart narrative insights
- Trend analysis — what went up, what went down, steepest inclines
- Country level comparisons with % differences

---

## 💡 Key Business Insights

1. **Germany has the highest churn rate at 49.71%** — despite having only 2,500 customers, it accounts for 39.96% of all exited customers
2. **France has the most customers (5,014)** but a relatively lower churn rate at 24.75%
3. **Age group 38–47 has the most inactive members (1,702)** — this is a high-risk segment
4. **Age group 28–37 has the most active members (2,074)** — most engaged customer segment
5. **Churn peaked in 2018 at 27.59%** — dropped to 12% in 2017 showing high volatility
6. **Total customers grew 20% between 2016 and 2019** — but exited customers also grew by 174.76%
7. **France vs Spain gap** — France had 4,204 more customers than exited customers — widest retention gap across all countries

---

## 🎯 Recommendations

| # | Recommendation | Expected Impact |
|---|----------------|----------------|
| 1 | Focus retention strategy on Germany — 49.71% churn is too high | Reduce overall churn significantly |
| 2 | Target age group 38–47 with re-engagement campaigns | Convert inactive to active members |
| 3 | Study what France is doing right and apply to Germany and Spain | Bring down churn in other regions |
| 4 | Investigate 2018 churn spike — what happened that year | Prevent repeat of 27.59% churn |
| 5 | Replicate growth pattern from May–Dec 2016 (103% growth in 7 months) | Sustainable customer growth |

---

## 🚀 How to Open This Project

1. Download **Power BI Desktop** for free from [powerbi.microsoft.com](https://powerbi.microsoft.com/desktop/)
2. Download the `.pbix` file from the `POWer Bi` folder in this repository
3. Open in Power BI Desktop — all data and visuals load automatically

---

## 📬 Contact

**Rajeev Kumar**
- 📧 Email: hireraajeev@gmail.com
- 💼 LinkedIn: [linkedin.com/in/reactwithrajeev](https://www.linkedin.com/in/reactwithrajeev/)
- 🐙 GitHub: [github.com/reactwithrajeev](https://github.com/reactwithrajeev)

---

> ⭐ If you found this project helpful, please give it a star!
