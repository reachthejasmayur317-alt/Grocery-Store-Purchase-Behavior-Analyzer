# Grocery-Store-Purchase-Behavior-Analyzer
A Data Storytelling Project using Python (Colab), Power BI & Tableau

This project analyzes supermarket sales data to uncover key business insights related to customer behavior, product performance, time-based shopping patterns, and store profitability.
The goal was to build a data-driven decision-making system with advanced visualization dashboards for storytelling.
Using Google Colab, the dataset was cleaned and enriched with:

✔ Feature Engineering

day_of_week

month

order_hour

is_weekend

basket_size

Revenue

Profit
df['Date'] = pd.to_datetime(df['Date'])
df['day_of_week'] = df['Date'].dt.day_name()
df['order_hour'] = pd.to_datetime(df['Time']).dt.hour
df['is_weekend'] = df['day_of_week'].isin(['Saturday','Sunday']).astype(int)
df['basket_size'] = df['Quantity']
df['Revenue'] = df['Sales']
df['Profit'] = df['gross income']
2. Power BI Dashboards
## 🏬 Page 1 — Store Performance Overview

Insights Included:

Total Revenue

Total Profit

Average Customer Ratings

Total Transactions

Revenue by Branch

Revenue by City

Product Line Performance

Payment Method Distribution

👥 Page 2 — Customer Behavior

Key Insights:

Revenue by Customer Type (Member vs Normal)

Average Basket Size

Gender-based revenue patterns

Product line preferences by customer type

Customer satisfaction across groups

⏰ Page 3 — Time Intelligence Dashboard

Visuals:

Sales by Day of Week

Sales by Hour

Weekend vs Weekday Analysis

Heatmap (Day × Hour × Revenue)

Peak shopping times

These visuals help identify ideal staffing hours, promotion timing, and product placement strategies.

📈 3. Tableau Dashboards

A complementary Tableau dashboard was built to showcase:

Geographic revenue view

Revenue by product category

Customer ratings story

City-wise profitability

Time series trends

🎯 Key Business Insights
🔹 Product Insights

Health & Beauty and Food & Beverages were top contributors to revenue.

“Home and lifestyle” offered high profit margins.

🔹 Customer Behavior

Member customers bought more items on average.

Males spent slightly more, but purchase frequency was similar.

🔹 Time Trends

Evenings (5 PM–8 PM) had peak revenue hours.

Weekends had higher average bill values.

🔹 Payment Trends

Credit Card, Cash, and E-Wallet usage was almost evenly distributed.
