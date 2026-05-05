# E-commerce User Behavior and Conversion Analysis

**Objective:** Analyze user behavior using clickstream data to identify conversion patterns, drop-off points, and opportunities to improve the user journey from product view to purchase.

## Diagnosing Conversion Patterns Across 75K+ Clickstream Events

**Dataset:** ~75K clickstream events and transactions from a simulated e‑commerce store  
https://www.kaggle.com/datasets/waqi786/e-commerce-clickstream-and-transaction-dataset
## 📊 Dataset Overview

| Metric        | Value                                                                |
| ------------- | -------------------------------------------------------------------- |
| Total Records | 74,000+                                                              |
| Unique Users  | 1000                                                                 |
| Products      | 8700+                                                                |
| Event Types   | page_view, product_view, add_to_cart, purchase, login, logout, click |

Dataset contains user interaction events across multiple sessions.

## Business Problem

The e-commerce platform generates high user activity with ~73,000 sessions, but lacks clear visibility into how user interactions translate into conversions and revenue.

Despite strong engagement, key decision-making gaps remain:

**Key Questions**

- Where does the conversion funnel break, and what causes drop-offs?
- Which products receive high views but low purchases?
- What user actions are most strongly associated with successful conversions?
- Which products contribute the most to overall revenue?
- How do user sessions differ between converting and non-converting behavior?
- Do repeat users (multiple sessions) show higher likelihood of purchase?
  
## This project investigates

- How users move through the funnel from product view to add to cart to purchase
- Which products have high visibility but low conversion rates
- How revenue is distributed across products and changes over time
- How users behave across sessions and what actions lead to successful purchases

## Key Analyses & Metrics

- **Product interactions:** Top products by views/clicks and interactions by category.  
- **Conversion funnel:** Session-level funnel from view → add-to-cart → purchase, with step-wise conversion and drop-off rates.  
- **Revenue analysis:** Revenue trend over time (daily/weekly) and top revenue-contributing products and categories.  
- **Product conversion:** View-to-purchase conversion rate per product, highlighting high-view low-conversion items.  
- **User behavior:** One-time vs repeat users, and comparison of session behavior for purchasing vs non-purchasing sessions.

## Data Understanding & Cleaning

The dataset was explored to understand its structure, event types, and relationships between users, sessions, and products.

Timestamp fields were converted into datetime format to enable time-based analysis such as session creation and trend analysis.

Missing values were examined across different event types, especially for fields that are only relevant to specific actions like purchases or cart events, ensuring accurate interpretation of user behavior.

Relationships between users, sessions, and products were validated using keys such as session_id, user_id, and product_id to ensure consistency before performing aggregations and analysis.

## Key Insights

User engagement is high, with users performing multiple actions per session and returning frequently. This indicates strong platform activity and interest.

The conversion funnel shows a high progression from product view to purchase within the dataset. While this suggests efficient movement through the funnel, it also indicates that the dataset may not fully capture real-world drop-offs.

Several products receive high user attention but have low purchase counts. These represent missed revenue opportunities and potential issues in pricing, product presentation, or user experience.

Revenue is concentrated among a smaller set of products, indicating that a few products drive a significant portion of business performance.

User actions such as product views and add-to-cart events are strongly associated with purchases, highlighting the importance of engagement-driven conversion.

## Business Recommendations

Improve conversion for low-performing products by optimizing pricing, product descriptions, and visual presentation. Adding customer reviews and trust signals can also improve purchase confidence.

Enhance the user journey by reducing friction in the add-to-cart to purchase stage. Simplifying checkout and improving user interface design can increase conversions.

Focus on high-performing products by promoting them through recommendations, featured listings, and targeted campaigns.

Leverage user engagement by implementing personalized recommendations and retargeting strategies for active users.

Improve data tracking by ensuring proper event sequencing and capturing more realistic user drop-offs across the funnel.

## Tools & Techniques

- Python (data cleaning, transformation, analysis)  
- Pandas (groupby, aggregations, joins, session‑level features)
- Matplotlib (funnel charts, trend lines, bar plots)
- Jupyter Notebook (exploratory analysis and storytelling)
