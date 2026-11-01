# Device Insurance Attach-Rate Analytics

> Store-level analysis of monthly device-insurance attach % across a multi-branch retail chain: branch and regional performance, seasonality, store risk flags, and expansion recommendations.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?logo=microsoftexcel&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?logo=tableau&logoColor=white)

## Overview
**Attach %** is the share of device customers who also buy an insurance plan (screen protection, extended warranty, accidental damage). A higher attach % means more revenue per device sold, so it is a key retail KPI.

This project analyses monthly attach % for **103 stores across 6 branches (Aug-Dec)** to answer:
- Which branches, regions and stores perform best, and which are at risk?
- How does performance change month to month?
- Where should the business expand, fix, or rationalise?

> Data is confidential and not included. Store names in the report are for illustration only.

## Approach
1. **Data prep:** loaded store x month attach % (Branch, Store Name, Aug-Dec) and checked structure and missing values.
2. **Derived columns:** Store Avg Attach, Branch Avg Attach, Active Months, Zero-Attach Months, Store Category, Risk Flag, Underperformance Flag, Region Type.
3. **Regional grouping:** North (Delhi NCR), West (Gujarat, Mumbai, Pune, Thane), South (Telangana).
4. **Analysis and visuals:** branch comparison, month-wise trends, store-level matrices and zero-attach detection (Python, Excel, Tableau).
5. **Recommendations** per branch and region.

## Key Findings
- **Seasonality:** November-December is the peak period; August is the lowest.
- **Pune:** the most stable branch, with consistent attach % across months, yet only 16 stores. It is the strongest candidate for expansion.
- **Delhi NCR:** the most profitable branch (44 stores, above-median performance, few zero-attach months). Upside remains in its weakest stores through campaigns and training.
- **Telangana:** 40 stores, but the lowest regional contribution. Several stores recorded **0% attach even in the November peak**, pointing to structural issues rather than seasonality.
- **Regions:** West contributes the most and South the least; North (Delhi NCR) is a high-intensity market where new initiatives should be piloted first.

## Recommendations
- Expand in **Pune**, and review its low-active-month stores first.
- Retain top Telangana stores and put chronic zero-attach stores through corrective action, then rationalise if there is no improvement.
- Use targeted staff training, incentive restructuring and sales scripts in underperforming stores.
- Pilot new services and campaigns in **Delhi NCR**.

## Repository Structure
```
├── report/        # Full analysis report (PDF)
├── notebooks/     # Python analysis
├── screenshots/   # Key charts
└── README.md
```

## Tools
Python (Pandas, Matplotlib) | Excel | Tableau

## Author
**Tishya Chauhan** | B.Sc. Data Analytics, DSEU | [GitHub](https://github.com/tishyachauhan)
