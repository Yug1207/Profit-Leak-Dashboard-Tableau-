# The Profit Leak Report: SuperStore Profit Dashboard (Tableau)

A Tableau dashboard that asks one question about a retailer: **where is the business losing money while sales look healthy?**

## What this is

My individual assignment for the 4th semester of the BS in Analytics and Sustainability Studies at TISS Mumbai. Instead of building charts first, I wrote the business questions first and picked each chart to answer one of them.

**Data:** Tableau's Sample Superstore dataset (a fictional retailer): 10,194 order lines from 2023 to 2026, across 3 customer segments, 4 regions, 17 product sub-categories and 542 cities.

## The four questions

1. **Discounts:** how does discounting affect profit margin?
2. **Products:** which sub-categories lose money while looking like they contribute?
3. **Segments and regions:** do certain customer types lose money in certain regions?
4. **Cities:** are the busiest cities also the most profitable?

## What is in the dashboard

- **KPI strip:** Total Sales, Total Profit, Average Discount Given, Loss Order Rate.
- **City map:** bubbles sized by sales, coloured by whether the city makes or loses money.
- **Discount impact chart:** profit margin by discount tier (None, Low, Medium, High).
- **Product treemap:** sub-categories sized by sales, coloured by margin.
- **Segment and region bar chart:** margin for every segment-region pair.
- **Filters** for segment, product profit status and discount profit status, which update the other charts.

Colour means the same thing everywhere: green is profitable, yellow is marginal, red is a loss.

## What the data shows

These figures were checked against the data inside the workbook.

- **$2.33M in sales, $292K in profit,** an average discount of **15.5%**, and **18.6% of transactions lose money**.
- **Discounts above 20% turn margins negative.** Average margin is 29.6% with no discount, 11.9% at low discounts, **-15.3% at medium** and **-77.4% at high**.
- **Three sub-categories lose money:** Tables (-8.5%), Bookcases (-3.2%) and Supplies (-2.5%). Paper (43.4%) and Labels (43.9%) are the most profitable.
- **No segment-region pair loses money overall,** but Consumer in the Central region is thin at 3.4%, and Home Office in the South is next at 6.2%.
- **118 of 542 cities lose money,** including large markets such as Philadelphia, Houston and Chicago.

## Calculated fields

Profit Margin %, Discount Tier, Loss Order Flag and Loss Order Rate, Product Profit Status, City Profit Status, Discount Profit Status, Days to Ship.


## Open it

Download `Tableau_Assignment.twbx` and open it in Tableau Desktop or Tableau Public (both free options exist). The data is packaged inside the file, so nothing else is needed.

## Author

**Yug Bhogi**, BS in Analytics and Sustainability Studies (2024-28), TISS Mumbai.
GitHub: [Yug1207](https://github.com/Yug1207)
