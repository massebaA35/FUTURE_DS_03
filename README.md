# FUTURE_DS_03
Marketing funnel &amp; conversion analysis using retail order data. Built a proxy funnel (Quantity = engagement, Discount = incentive, Profit = conversion, Region = channel) with Excel dashboard + Power BI report, tracking drop-off across 4 stages and conversion rates by region/category.
# Marketing Funnel & Conversion Performance Analysis

## Overview
This project analyzes marketing funnel and conversion performance using a 
retail order-level dataset that lacked native lead/channel funnel data. 
Since no direct "leads → opportunities → customers" fields existed, a 
**proxy funnel** was constructed using available order attributes:

- **Quantity** → engagement/buyer intent
- **Discount** → negotiation/incentive needed to close
- **Profit** → successful, value-generating conversion
- **Region** → channel proxy

## Funnel Stages
1. **Stage 1 – Top of Funnel**: All orders placed
2. **Stage 2 – Engaged**: Orders with Quantity ≥ 6
3. **Stage 3 – Incentivized**: Engaged orders with Discount > 0
4. **Stage 4 – Converted**: Incentivized orders with Profit > 0

## Deliverables
- 📊 **Excel Dashboard** (`Marketing_Funnel_Conversion_Analysis.xlsx`) — 
  live formulas (COUNTIFS), funnel/region/category breakdowns, charts, 
  and insights
- 📈 **Power BI Report** — funnel visual, KPI cards, region/category 
  conversion bar charts, interactive slicers (Region, Category, Segment)

## Key Insights
- Largest drop-off occurs at Stage 1 → 2 (~50% of orders fall below the 
  engagement threshold)
- ~61% of engaged orders still required a discount to progress
- Discounted, engaged orders convert to profit ~85% of the time
- South region underperforms (~25% conversion) vs Central/East (~27%)

## Tools Used
Excel (formulas, charts) · Power BI (DAX measures, funnel visual, slicers) · Python/pandas (initial data exploration)
