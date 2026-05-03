# District-Wise Sectoral Analysis of Indian States

SQL-based economic analysis of primary, secondary, and tertiary sector contributions across Indian districts, visualised using Looker Studio.

![SQL](https://img.shields.io/badge/SQL-4479A1?logo=mysql&logoColor=fff&style=flat-square)
![Looker Studio](https://img.shields.io/badge/Looker_Studio-4285F4?logo=google&logoColor=fff&style=flat-square)
![Excel](https://img.shields.io/badge/Excel-217346?logo=microsoft-excel&logoColor=fff&style=flat-square)
![States](https://img.shields.io/badge/States-20-orange?style=flat-square)
![Districts](https://img.shields.io/badge/Districts-307-blue?style=flat-square)

---

## Problem Statement

India's economic growth is unevenly distributed across districts and states. Understanding which sectors — primary (agriculture), secondary (manufacturing), or tertiary (services) — dominate specific regions is critical for policy-making, investment decisions, and business expansion strategies. This project analyzes district-level sectoral data across Indian states to uncover patterns, disparities, and growth opportunities.

---

## Project Highlights

- Analyzed 2,149 records across 307 districts and 20 Indian states (2007–2013)
- Wrote 20 SQL queries covering filtering, aggregation, joins, window functions, subqueries, and trend analysis
- Identified Gurgaon as the highest growth district in the tertiary sector over a 5-year period (234.5% growth rate)
- Found Tamil Nadu as the top tertiary sector contributor at current prices in 2010
- Built an interactive Looker Studio dashboard for real-time exploration of sector performance

---

## Dataset

| Field | Details |
|---|---|
| Source | District-level economic data — Indian states |
| Records | 2,149 rows |
| Districts | 307 |
| States | 20 |
| Time Period | 2007–2013 (base year 2004) |
| Sectors | Primary, Secondary, Tertiary |
| Metrics | Constant prices, current prices, sector shares (%) |

**States covered:** Andhra Pradesh, Assam, Bihar, Chhattisgarh, Gujarat, Haryana, Himachal Pradesh, Jharkhand, Karnataka, Kerala, Madhya Pradesh, Maharashtra, Orissa, Punjab, Rajasthan, Tamil Nadu, Telangana, Uttar Pradesh, Uttarakhand, West Bengal

---

## Tech Stack

| Category | Tools |
|---|---|
| Data Analysis | SQL (MySQL) |
| Visualisation | Looker Studio |
| Validation | Excel |

---

## SQL Queries Performed

| # | Query Type | Description |
|---|---|---|
| 1 | Basic Query | Retrieve all data for a specific state |
| 2 | Filtering | Districts with total contribution above threshold |
| 3 | Aggregation | Total primary sector contribution by district and year |
| 4 | Join Operation | State-wise analysis combining district and state data |
| 5 | Growth Calculation | Year-on-year secondary sector growth for a district |
| 6 | Trend Analysis | District with highest tertiary sector growth over 5 years |
| 7 | Group By | Total secondary sector contribution per state |
| 8 | Comparison | Per capita income comparison between two districts |
| 9 | Ranking | Rank districts within a state by total constant prices |
| 10 | Sector Filtering | Districts where primary sector share exceeds 20% |
| 11 | Sector Performance | Average tertiary sector share per state over time |
| 12 | Max-Min Analysis | Highest and lowest economic districts in a state |
| 13 | Percentage Contribution | Secondary sector percentage contribution per district |
| 14 | Conditional Filtering | Districts where tertiary share > secondary share |
| 15 | Multi-Condition | Districts where both primary and secondary shares > 30% |
| 16 | Time Series | Total contribution trend over time for a district |
| 17 | Subquery | State with highest tertiary sector contribution in a year |
| 18 | Distinct Query | All unique states in the dataset |
| 19 | Join and Aggregate | Total economic contribution per district for a state/year |
| 20 | Window Function | Cumulative primary sector total for a district over years |

---

## Key Findings

- **Gurgaon** recorded the highest tertiary sector growth rate of **234.5%** over a 5-year period
- **Tamil Nadu** was the top tertiary sector contributor at current prices in 2010
- **Karnataka** had the highest total secondary sector contribution (Rs 4,736,325 million) among all states
- **Jabalpur** showed consistent growth in total current prices from Rs 91,837M (2007) to Rs 188,542M (2012) — a 2x increase in 5 years
- **Bastar** had the highest primary sector share at 36.52% — indicating strong agricultural dependency
- Districts like **Dewas** and **Sarguja** had both primary and secondary sector shares above 30%, indicating a mixed economic structure
- Tertiary sector dominance was concentrated in urban districts; rural districts showed higher primary sector dependency

---

## Project Structure
├── Dataset.csv                  # Raw district-wise sectoral data
├── Analysis.sql                 # 20 SQL queries with comments
├── Dashboard.png                # Looker Studio dashboard screenshot
├── Project Report.pdf           # Detailed project report
├── Presentation Overview.pptx   # Summary presentation
└── README.md

---

## How to Run

```sql
-- Load the dataset into MySQL
CREATE DATABASE sectoral_analysis;
USE sectoral_analysis;

-- Import Dataset.csv as table: district_sectorial
-- Then run queries from Analysis.sql
```

---

## Dashboard Preview

![Dashboard](Dashboard.png)

---

## Author

**Harshit Saraf**
PGDM Business Analytics — Vivekanand Education Society's Business School, Mumbai
[LinkedIn](https://www.linkedin.com/in/harshit-saraf-h9) · [GitHub](https://github.com/Happy295-hue)
