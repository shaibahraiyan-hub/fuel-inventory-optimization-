# Fuel Inventory Optimization Analysis

**Tools:** Python, Pandas, NumPy, Matplotlib  
**Context:** Graduate coursework — Johns Hopkins Carey Business School

---

## Overview

Analyzed 1+ year of real-world fuel purchasing and inventory data across 8 gas station locations to evaluate current replenishment practices and propose cost-saving ordering strategies.

The dataset included fuel level readings, invoices, tank specifications, and station locations — merged and cleaned across 5 CSV files.

---

## Business Questions Addressed

### 1. Evaluate Current Inventory Management
- Concatenated and cleaned fuel level data from two datasets (500K+ rows)
- Merged tanks, locations, and invoice data into a unified analytical dataset
- Visualized per-tank fuel levels over time with a 10% stockout threshold
- Identified tanks at risk of stockout vs. those with effective inventory management
- Calculated discount savings achieved per station (Stations 1–8) based on supplier volume tiers

### 2. Recommend Improved Ordering Strategies
- Determined maximum applicable discount tier based on total tank capacity per location and fuel type
- Calculated a 7-day safety stock threshold using average daily consumption
- Found that **all stations currently order below the 15,000L minimum** required to earn any volume discount (0¢/L)
- Modeled optimized order quantities to reach higher discount tiers (up to 4¢/L)

### 3. Identify the Best Day for Fuel Orders
- Computed price-per-liter for each invoice
- Applied IQR-based outlier filtering to remove extreme values
- Analyzed price distribution by day of week
- Identified **Thursday** as the optimal purchase day (mean price: $1.1036/L)
- Estimated **~$12.3M CAD** in additional savings if purchases were consistently made on Thursdays

### 4. Evaluate the Feasibility of Adding Tanks
- Modeled the impact of adding a 30,000L tank ($100,000 CAD cost) at each location
- Calculated annual extra savings from unlocking higher discount tiers
- Performed 5-year NPV analysis (2% discount rate)
- **Station 1** identified as top candidate: NPV ~$124K > $100K tank cost ✅

---

## Key Findings

| Analysis | Finding |
|---|---|
| Current discount captured | $0 — all stations below 15,000L threshold |
| Potential discount tier | 4¢/L if ordering to full tank capacity |
| Best purchase day | Thursday ($1.1036/L avg) |
| Projected day-of-week savings | ~$12.3M CAD |
| Best tank expansion candidate | Station 1 (NPV: ~$124K) |



## Technical Skills Demonstrated

- Data cleaning & merging (Pandas)
- Time series visualization (Matplotlib)
- Outlier detection (IQR filtering)
- Discount tier modeling
- NPV / cost-benefit analysis
- Inventory policy recommendations
