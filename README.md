# E-commerce User Behavior & Conversion Funnel Analysis

**Objective:** Analyze user behavior using clickstream data to identify conversion patterns, drop-off points, and opportunities to improve the user journey from product view to purchase.

**Tools:** Python · Pandas · Matplotlib · Jupyter Notebook

## Diagnosing Conversion Patterns Across 75K+ Clickstream Events

**Dataset:** ~75K clickstream events and transactions from a simulated e‑commerce store  
https://www.kaggle.com/datasets/waqi786/e-commerce-clickstream-and-transaction-dataset

This analysis examines how users interact with an e-commerce platform and how their actions translate into conversions. Using clickstream data, the project tracks user journeys across key events such as product views, add-to-cart actions, and purchases. By reconstructing user sessions and analyzing behavior across these stages, it identifies conversion patterns, user engagement trends, and critical drop-off points within the funnel. The goal is to uncover actionable insights to improve user experience, optimize the conversion process, and enhance overall business performance.

## Business Problem

E-commerce platforms need to understand user behavior and conversion dynamics to optimize engagement, improve the user journey, and increase revenue.

This project addresses the following key business questions:

**Product Engagement:**
- Which products receive the highest user interactions (views/clicks)?
- Are high-engagement products effectively converting into purchases?

**Conversion Funnel Analysis:**
- How do users progress through the funnel (view → add-to-cart → purchase)?
- At which stage does the largest drop-off occur?
- Which stage requires optimization to improve conversion rates?

**Revenue Insights:**
- How does revenue evolve over time based on purchase activity?
- Which products contribute the most to overall revenue?
  
**Product Conversion Performance:**
- Which products have high visibility but low conversion rates?
- Which products demonstrate strong conversion performance?
  
**User Behavior Analysis:**
- What distinguishes repeat users from one-time users?
- Which user actions are most strongly associated with successful conversions? 

## Tools & Techniques

- Python (data cleaning, transformation, analysis)  
- Pandas (groupby, aggregations, joins, session‑level features)
- Matplotlib (funnel charts, trend lines, bar plots)
- Jupyter Notebook (exploratory analysis and storytelling)

## Key Analyses & Metrics

- **Product interactions:** Top products by views/clicks and interactions by category.  
- **Conversion funnel:** Session-level funnel from view → add-to-cart → purchase, with step-wise conversion and drop-off rates.  
- **Revenue analysis:** Revenue trend over time (daily/weekly) and top revenue-contributing products and categories.  
- **Product conversion:** View-to-purchase conversion rate per product, highlighting high-view low-conversion items.  
- **User behavior:** One-time vs repeat users, and comparison of session behavior for purchasing vs non-purchasing sessions.

## Data Understanding & Cleaning

- Inspected dataset structure with `info()` and `describe()` to understand data types, ranges, and basic distributions.  
- Converted timestamp columns to proper `datetime` format and derived date/time-based features (day, hour).  
- Checked and handled missing values by event type (e.g., columns that only apply to purchase/cart events).  
- Verified relationships between tables (sessions, events, transactions) using keys such as `session_id`, `user_id`, and `product_id`.
