# Woolworths-Executive-Sales-Dashboard
## Project Objective
To analyze Woolworths transaction data and uncover genuine product purchase relationships — moving beyond standard revenue/category reporting to identify which products are actually bought together — so that merchandising and marketing decisions (bundling, cross-selling, store layout, promotions) can be based on statistical evidence rather than assumption.

## Dataset used
- <a href="https://github.com/padhigeetha-cpu/Woolworths-Executive-Sales-Dashboard/blob/main/Woolies%20merchandise%20-%20Data.xlsx"> Woolworths Merchandise data </a>

## Question (KPIs)
- What is the total revenue and total number of orders? (KPI cards)
- What is the average order value? (KPI = Total Revenue ÷ Total Orders)
- How do sales and orders compare month-over-month? (dual-axis line/bar chart)
- Is order volume growing faster than revenue, or slower? (tells you if avg order value is rising or falling)
- What is the top-selling product by revenue? (KPI card)
- What is the top-selling product by quantity/units? (KPI card — often different from top revenue product)
- Which products contribute the most to total revenue  (sorted bar chart)
- Which products are underperforming and might need to be discontinued or promoted? (bottom-ranked bar chart)
- Is there a mismatch between high-volume and high-revenue products? (scatter plot of quantity vs. revenue)
- Which category drives the most revenue? (bar chart by category)
- Which products are most frequently bought together? (correlation matrix / scatter plot)
- What's the average number of items per order (basket size)? (KPI)

## Dashboard 
- <a href="https://github.com/padhigeetha-cpu/Woolworths-Executive-Sales-Dashboard/blob/main/woolworths%20correlation%20dashboard.png"> view Dashboard </a>
- <a href="https://github.com/padhigeetha-cpu/Woolworths-Executive-Sales-Dashboard/blob/main/woolworths%20product%20correlation.png"> view product correlation </a>
<img width="576" height="717" alt="image" src="https://github.com/user-attachments/assets/da23a95c-9ab5-4f84-b357-7c38c9efe91b" />

## Solution Approach
Built an executive sales dashboard in Excel combined with a statistical correlation analysis of transaction-level order data:

- Consolidated raw order data and calculated revenue and quantity sold by product category.
- Built a 10x10 product correlation matrix using Excel's CORREL function across all product pairs, with conditional formatting to visually flag strong (green) and weak/negative (red) relationships.
- Validated the three most business-relevant correlations — Milk & Diapers, Diapers & Wet Wipes, and Pasta & Pasta Sauce — with scatter plots and trendlines to confirm the matrix results weren't statistical noise.
- Packaged revenue, volume, and correlation findings into a single executive KPI dashboard for quick stakeholder consumption.

## Key Outcomes
- Identified Pasta & Pasta Sauce (r = 0.96) as a near-perfect, very strong purchase pair.
- Identified Diapers & Wet Wipes (r = 0.70) as a strong cross-category relationship.
- Ruled out Milk & Diapers (r = 0.09) as having no meaningful correlation — despite both being high-frequency household categories, they are not driven by the same shopping trips.
- Revealed a revenue/volume mismatch: Diapers drove the highest revenue ($23,625) on relatively low volume (1,125 units), while Wet Wipes drove the highest volume (4,045 units) on lower per-unit value — two different commercial roles requiring different strategies.
- Delivered a single dashboard view combining revenue ($117,124 total), volume (20,720 units), and correlation insight for non-technical stakeholders.


## Recommendations
- Bundle or co-locate Pasta and Pasta Sauce in-store and in promotions — the data supports this as a near-guaranteed joint purchase, making it a low-risk, high-confidence merchandising move
- Cross-promote Diapers with Wet Wipes (e.g. baby-care bundle discounts, adjacent shelf placement) to capture the strong existing purchase relationship and lift average basket size
- Avoid bundling Milk with Diapers — the near-zero correlation suggests customers don't treat these as a shared shopping occasion, so joint promotions here are unlikely to move volume
- Treat Diapers as a margin/revenue driver and Wet Wipes as a volume/traffic driver in category planning, rather than applying the same pricing or promotional logic to both
- Extend the correlation methodology to the full product catalog (beyond these 10 categories) to systematically surface additional bundling opportunities rather than relying on a handful of manually tested pairs

## Tools & Techniques
Microsoft Excel · Pivot Tables & Pivot Charts · CORREL Function · Conditional Formatting · Scatter Plot & Trendline Analysis · KPI Dashboard Design · Market Basket Analysis
