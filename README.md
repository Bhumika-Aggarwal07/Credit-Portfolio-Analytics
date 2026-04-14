# Credit Portfolio Analytics 

> Analysing customer risk, spending behaviour across a retail bank's credit card portfolio using Python and Pandas.

![Python](https://img.shields.io/badge/Python-3.13-blue?style=flat-square&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=flat-square&logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualisation-4c72b0?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

---

## Problem Statement

A mid-size retail bank wants to evaluate the health of its credit card portfolio. The business needs to:
- Identify **high-risk customers** before they default
- Understand **spending behaviour** across customer segments
- Find customers who are under-charged or poorly matched to their card tier
- Generate **actionable recommendations** to reduce credit losses and grow revenue

---

## Dataset

Three relational tables — synthetic banking data representing a realistic portfolio:

| Table | Description | Size |
|---|---|---|
| `credit.csv` | Customer master — demographics, card type, credit limit | 100 rows × 8 cols |
| `spend.csv` | Monthly spend transactions by category | 1,500 rows × 5 cols |
| `repayment.csv` | Monthly repayment amounts | 1,523 rows × 5 cols |

---

## Key Findings

| # | Finding | Business Implication |
|---|---|---|
| 1 | ~45% of customers are **Overpaid** — repayments exceed spending | Strong candidates for credit limit upgrades and premium card offers |
| 2 | **Salaried Private sector** has the highest High-Risk concentration (~54%) | Stricter income verification needed at underwriting stage |
| 3 | **Platinum & Silver cards** show ~43% High-Risk customers | Approval criteria for these tiers needs a review |
| 4 | **Gold card users** have the lowest High-Risk rate (~16%) | Most financially stable segment — prioritise for retention and loyalty rewards |
| 5 | **26–35 age cohort** drives the highest spend volumes | Key growth segment for targeted EMI and lifestyle offers |
| 6 | Persistent monthly **Coverage Gaps** indicate structural repayment lag | Pre-due-date reminders could significantly improve repayment rates |
| 7 | Spend concentrated in **2–3 categories** | Opportunity for merchant co-brand partnerships and category-specific cashback |

---

## Analysis Sections

1. Libraries & Setup
2. Data Loading & Overview
3. Data Cleaning & Preprocessing
4. Customer Risk Classification (Utilisation Ratio + Repayment Coverage)
5. Spending Behaviour by Segment, Age Group, and Card Type
6. Repayment Analysis & Coverage Gap Detection
7. Correlation Analysis — Spend vs Repayment by Risk Tier
8. Category-wise Spend Breakdown
9. Key Business Insights
10. Business Recommendations (Immediate / Medium-Term / Growth)

---

## Business Recommendations Summary

**Immediate (Risk Mitigation)**
- Auto-flag and freeze over-limit accounts until partial repayment is made
- Prioritise collections for High-Risk customers in the Salaried Private segment
- Reduce credit limits for customers with Utilisation Ratio > 1.0

**Medium-Term**
- Strengthen underwriting for Platinum and Silver cards with higher income verification
- Introduce early repayment incentives (e.g., 1% cashback for full pre-due-date payment)
- Implement monthly trend alerts for customers whose repayment-spend gap widens for 2+ consecutive months

**Growth**
- Upsell credit limit increases to Overpaid customers who show strong repayment capacity
- Establish co-brand merchant partnerships in the top 2–3 spending categories
- Launch lifecycle marketing campaigns targeting the 26–35 age cohort

---

## Tech Stack

- **Python 3.13** — core analysis
- **Pandas** — data manipulation, merging 3 relational tables, groupby aggregations
- **NumPy** — numerical calculations
- **Matplotlib + Seaborn** — visualisations (bar charts, heatmaps, scatter plots, trend lines)
- **Jupyter Notebook** — structured narrative analysis

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/Bhumika-Aggarwal07/Credit-Banking-Project-Pandas.git
cd Credit-Banking-Project-Pandas

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Launch notebook
jupyter notebook notebook/Credit_Banking_Project_v2.ipynb
```

The data files are in the `data/` folder. No external API keys or downloads needed.

---

## Project Structure

```
Credit-Banking-Project-Pandas/
├── data/
│   ├── credit.csv
│   ├── spend.csv
│   └── repayment.csv
├── notebook/
│   └── Credit_Banking_Project_v2.ipynb
└── README.md
```

---

## Resume Bullet Points

- Analysed a 100-customer retail banking credit portfolio across 3 relational tables (3,000+ rows) using Python and Pandas to identify risk segments, spending patterns, and revenue leakage
- Built a customer risk classification framework using Utilisation Ratio and Repayment Coverage metrics; found that Platinum/Silver cardholders hold ~43% high-risk customers — surfaced a structural underwriting gap
- Delivered 7 data-driven business insights and 9 actionable recommendations across risk mitigation, medium-term operations, and growth strategy

---

## Author

**Bhumika Aggarwal** — 1st Year BTech CSE  
[LinkedIn](https://www.linkedin.com/in/bhumika-aggarwal-5a89ab379) · [GitHub](https://github.com/Bhumika-Aggarwal07)
