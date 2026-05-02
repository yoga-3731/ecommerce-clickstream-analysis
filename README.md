# Clickstream User Behavior & Conversion Funnel Analysis

**Goal:** Analyze e‑commerce clickstream data to reconstruct user sessions, understand behavior, and measure conversion across the view → cart → purchase funnel.

## Reconstructing User Sessions & Analyzing Conversion Funnel in Clickstream Data

Tools: Python · Pandas · Matplotlib · Jupyter Notebook

Dataset: ~75K clickstream events and transactions from a simulated e‑commerce store  
https://www.kaggle.com/datasets/waqi786/e-commerce-clickstream-and-transaction-dataset

## Business Problem

E‑commerce platforms need to understand how users interact with their system in order to improve engagement and conversion rates.
This project answers the following key business questions:
1. Which products receive the highest user interactions (views/clicks)?  
2. How do users move through the funnel (view → cart → purchase)?  
   - Where is the largest drop-off?  
   - Which stage needs improvement?  
3. How does revenue change over time based on purchase events?  
   - Which products contribute most to revenue?  
4. Which products have high views but low purchases?  
   - Which products have the best conversion rates?  
5. How do users behave on the platform?  
   - Are there repeat users?  
   - What actions are associated with purchases?  

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
