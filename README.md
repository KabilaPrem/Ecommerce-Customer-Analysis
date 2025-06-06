### 🛍️ E-commerce Customer Journey Analysis

**Description:**  
Developed an interactive Power BI dashboard to analyze customer behavior and product trends using an e-commerce dataset from Kaggle. The project focused on transforming raw data into actionable insights to drive marketing and product decisions.

**Tools & Technologies Used:**  
- Excel (Data Cleaning, Pre-checks for nulls/duplicates)
- Python (Pandas for cleaning, type conversion, outlier removal)
- MySQL (SQL Queries, Joins, Aggregations)
- Power BI (Data Visualization, Slicers, KPIs)

**Key Features:**
- Cleaned and structured raw data using Python (`pandas`)
- Calculated KPIs such as:
  - Total Revenue
  - Average Order Value (AOV)
  - Repeat Purchase Rate
  - Customer Segmentation

## Data Analysis Using SQL
- Used MySQL to perform advanced queries for sales insights like
Below are some of the key SQL queries used in the project:
### Sum of Order Price:
```sql
select sum(order_price_inr) from dup_ecomm;
```
### Average Price:
```sql
select avg(order_price_inr) from dup_ecomm;
```
### Percentage of peoples who didn't use discounts:
```sql
SELECT 
    (COUNT(CASE WHEN discount_applied= "no" THEN customer_id END) * 100.0 / COUNT(customer_id)) AS percentage_without_discount
FROM dup_ecomm;
```
### Sum of order value based on items:
```sql
select sum(Order_Price_INR) from dup_ecomm group by Item_Purchased;
```

- Built a Power BI dashboard showing:
  - Product performance
  - Regional sales
  - Customer engagement trends
- Proposed business strategies:
  - Reduce pointless discounts
  - Boost subscribers over unsubscribers
  - Create advertising for repeat customers

📊 **Key Learnings**:
- Data cleaning & transformation
- SQL query writing for business insights
- Power BI visualization techniques
- Data modeling best practices


