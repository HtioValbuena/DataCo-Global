# DataCo Supply Chain Analysis
**Tool:** Power BI | **Dataset:** DataCo Smart Supply Chain (Kaggle)

## Business Problem
DataCo Global needed to understand why a significant portion of their orders 
were arriving late, which markets and shipping modes were most affected, 
and where profitability was being lost across their global supply chain.

## Key Findings
- **54.8%** of all orders arrive late — concentrated in First Class shipping (highest late delivery rate)
- Late delivery rate is consistent across all global markets (~50%), suggesting 
  a systemic issue with delivery time estimation rather than a regional logistics problem
- Q4 shows the highest late delivery rate, coinciding with peak sales season

## Dashboard Pages
| Page | Business Question |
|------|------------------|
| Logistics Performance | Where and why are deliveries failing? |
| Profitability | Which products and markets are actually profitable? |
| Sales & Products | What sells most and where? |
| Customer Analysis | Who buys and how do they behave? |

## Data Model
Star schema with 1 fact table and 4 dimension tables:
- **Fact_Orders** — 180,519 transactions
- **Dim_Product** — 118 unique products (Department → Category → Product hierarchy)
- **Dim_Geography** — Global markets (Market → Region → Country → State → City hierarchy)
- **Dim_Date** — 2015–2018 date table with time intelligence
- **Dim_Customer** — Customer segments and locations

## DAX Measures
13 custom measures including Late Delivery Rate %, Profit Margin %, 
Shipping Delay, and Avg Order Value.

## Status
🚧 In progress — Logistics Performance page complete
