# Coke-sales-analysis

## 📌 Project Description
This project analyzes Coca-Cola sales data across key American retailers using Excel. The objective is to extract actionable insights from transactional and operational metrics — total sales, units sold, and operating margin — to evaluate regional performance, retailer efficiency, and sales trends, and to identify strengths and opportunities for improvement.

**The analysis aims to understand:**
- How Coca-Cola sales vary by retailer, region, and time
- The relationship between pricing, volume, and profitability
- Trends in operating margins across different markets

**Business question:** *How can Coca-Cola optimize sales and profitability across U.S. retailers?*

---

## 📂 Dataset Overview
| Detail | Value |
|---|---|
| File | `Coke-sales-analysis-solution.xlsx` |
| Records | 3,888 transactions |
| Time period | Jan–Dec 2021 |
| Retailers | Sodapop, BevCo, FizzySip, DreamCo |
| Regions | Northeast, Midwest, South, Southeast, West |
| Cities covered | 52 |
| Brands | Coca-Cola, Diet Coke, Sprite, Fanta, Powerade, Dasani Water |
| Columns | Retailer, Retailer ID, Invoice Date, Region, State, City, Beverage Brand, Price per Unit, Units Sold, Total Sales, Operating Profit, Operating Margin, Month |
| Workbook sheets | `Data`, `Beginner`, `Intermediate`, `Advanced`, `Additional Analysis` |

---

## 🧹 Data Preparation
- Loaded and reviewed the multi-sheet Excel workbook, checking each sheet's purpose before analysis
- Standardized column headers (removed noisy/merged header rows above the actual data table)
- Confirmed categorical fields (Brand, Region, Retailer, City) used consistent naming with no duplicates/typos
- Verified **Invoice Date** was recognized as a proper date field and **Month** was correctly derived from it
- Confirmed numeric fields (Price per Unit, Units Sold, Total Sales, Operating Profit, Operating Margin) were formatted as currency/number/percentage, not text
- Checked for missing values — none found in core metric columns
- Structured the cleaned table as an Excel Table for reliable PivotTable refresh

---

## 💰 Sales & Profitability Analysis

**By Brand** (Total Sales | Units Sold | Avg. Margin)
| Brand | Total Sales | Units Sold | Avg Margin | Notes |
|---|---|---|---|---|
| Coca-Cola | $2.02M | 4.13M | 38.7% | Highest sales AND strong margin — flagship product |
| Dasani Water | $1.73M | 3.00M | 38.5% | Highest profit per unit — premium pricing |
| Diet Coke | $1.48M | 3.00M | 34.2% | Lowest average margin of all brands |
| Sprite | $1.24M | 2.70M | 34.9% | Steady, mid-tier performer |
| Powerade | $1.19M | 2.12M | 35.3% | Niche sports-drink segment, lower volume |
| Fanta | $1.03M | 2.19M | 36.2% | Lowest sales — driven by low volume, not price |

**By Region**
| Region | Total Sales | Notes |
|---|---|---|
| West | $2.84M | Highest — broadest retailer footprint (FizzySip + DreamCo, 13 cities incl. LA, SF) |
| Northeast | $1.79M | Sodapop-only, large city count |
| Southeast | $1.62M | Sodapop-only, fewer cities |
| South | $1.29M | BevCo-only |
| Midwest | $1.15M | Lowest — smaller markets despite similar city count to West |

**By Retailer**
| Retailer | Total Sales | Avg Margin | Notes |
|---|---|---|---|
| Sodapop | $4.40M (51%) | 36.4% | Highest sales — widest distribution (31 cities) |
| FizzySip | $2.58M | 32.9% | Second-largest, thinnest average margin |
| BevCo | $1.29M | 40.6% | Smaller scale but **most profit-efficient** |
| DreamCo | $0.40M | 38.3% | Lowest sales — only 2 cities, but healthy margin |

**Price vs. Volume:** Higher-priced items (Dasani Water, Powerade) sell fewer units but yield more profit per unit; Coca-Cola balances mid-range pricing with the highest volume, which is why it leads on total revenue.

---

## 📅 Time-Based Analysis
| Period | Sales | Why |
|---|---|---|
| **July** (peak) | $1.04M | Summer heat drives cold-beverage demand |
| **December** (peak) | $1.05M | Holiday season boosts purchases |
| **Feb–Mar** (trough) | ~$485K | Post-holiday slowdown + cold weather |

The trend is **bimodal** — two demand peaks (summer + holidays) with a spring dip — useful for planning inventory and promotions around these windows.

---

## 📊 Data Visualization
Built directly in the workbook using PivotCharts:
- **Bar charts** — Sales by Retailer, Sales by Month (Beginner sheet)
- **Pie charts** — Sales share by Region, Retailer, and Brand; Units Sold by Brand (Beginner sheet)
- **Line charts** — Monthly sales trend by Brand, Regional sales trend by Brand (Intermediate/Advanced sheets)
- **PivotTables + Slicer** — on the Intermediate sheet, allowing interactive filtering by Brand/Region/Retailer

---

## 💡 Insights & Recommendations
1. **Coca-Cola** is the strongest brand on both volume and margin — keep it central to strategy.
2. **Fanta** underperforms due to low demand, not pricing — a marketing/distribution push is a better lever than a discount.
3. **Dasani Water** is the most profit-efficient brand per unit — worth expanding shelf space.
4. **Sodapop drives 51% of total revenue** — a concentration risk; diversifying retailer partnerships would reduce exposure.
5. **BevCo runs the most efficient margin (40.6%)** of any retailer — a model worth replicating elsewhere.
6. **Regional and retailer totals are driven largely by footprint size** (number of cities/markets covered) rather than proof of stronger regional demand — worth normalizing by city count or population for a fairer comparison.
7. Plan **inventory and promotions around July and December peaks**, and expect a natural dip in Feb–Mar.

---

## 🛠 Tools Used
Microsoft Excel — PivotTables, PivotCharts, Slicers, formulas, data cleaning

