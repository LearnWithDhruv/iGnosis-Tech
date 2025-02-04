# Customer Profit Analysis

## Overview
This project aims to analyze customer transactions and purchasing behavior to identify:
1. The top 3 most profitable products.
2. The most loyal customer segments based on spending and purchase frequency.
3. Insights into customer behavior and recommendations for targeted marketing strategies.

## Dataset
The analysis is based on two datasets:
- **`transaction_data.csv`**: Contains customer transactions with product details and sales data.
- **`purchase_behaviour.csv`**: Contains customer demographic information, including life stage and spending category.

## Methodology
### Step 1: Data Loading and Exploration
- Read both datasets using pandas.
- Display sample data to understand structure and attributes.

### Step 2: Identifying Top 3 Most Profitable Products
- Group transactions by product number (`PROD_NBR`) and name (`PROD_NAME`).
- Calculate total revenue (`TOT_SALES`) per product.
- Sort and retrieve the top 3 products.

### Step 3: Identifying Most Loyal Customer Segments
- Group transactions by customer loyalty card number (`LYLTY_CARD_NBR`).
- Calculate total spending and purchase frequency for each customer.
- Merge with demographic data (`purchase_behaviour.csv`).
- Group by `LIFESTAGE` and `PREMIUM_CUSTOMER` to find the most frequent and high-spending customer segments.

### Step 4: Data Visualization
- Bar chart of **top 3 most profitable products**.
- Bar chart of **most loyal customer segments** by life stage and premium category.

### Step 5: Summary of Findings
- **Most profitable products generate the highest revenue**.
- **Older families** across all premium categories are the most loyal customers.
- Older families tend to purchase frequently and spend more per transaction.
- **Marketing Recommendation**: Personalized strategies targeting older families can boost revenue.

## How to Run the Analysis
1. Install required dependencies:
   ```sh
   pip install pandas matplotlib seaborn
   ```
2. Run the script:
   ```sh
   python customer_profit_analysis.py
   ```
3. Review the printed insights and visualizations.

## Results
The final output includes:
- **Printed insights** on top products and customer segments.
- **Visualizations** of key findings.
- **A summary report** with business recommendations.

## Future Improvements
- Expand analysis to seasonal trends in purchasing behavior.
- Implement a recommendation system for product suggestions.
- Explore customer retention strategies based on purchase history.

