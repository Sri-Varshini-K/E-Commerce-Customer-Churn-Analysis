# E-Commerce Customer Churn Analysis Using MySQL

## Project Overview

Customer churn is a major challenge for e-commerce businesses aiming to maintain customer satisfaction and long-term profitability. This project uses MySQL to analyze historical customer data, identify churn patterns, and explore the factors associated with customer attrition.

The analysis focuses on customer tenure, payment preferences, satisfaction scores, purchase behavior, complaints, cashback amounts, and order patterns to generate insights that can support customer retention strategies.

## Project Objectives

- Clean and standardize customer data.
- Handle missing values and outliers.
- Transform existing columns and create meaningful new attributes.
- Analyze active and churned customer behavior.
- Identify patterns in payment methods, order categories, and customer satisfaction.
- Examine the relationship between customer complaints and churn.
- Combine customer and return information using SQL joins.

## Tools & Technologies

- **Database:** MySQL
- **Query Language:** SQL
- **Key Concepts:** Data Cleaning, Data Transformation, Data Exploration, Aggregate Functions, GROUP BY, HAVING, Subqueries, and Joins

## Project Workflow

### 1. Data Cleaning

- Impute missing numerical values using the mean.
- Fill missing categorical or count values using the mode.
- Remove rows where `WarehouseToHome` exceeds 100.
- Standardize preferred login devices, order categories, and payment modes.

### 2. Data Transformation

- Rename `PreferedOrderCat` to `PreferredOrderCat`.
- Rename `HourSpendOnApp` to `HoursSpentOnApp`.
- Create `ComplaintReceived` to identify customers who submitted complaints.
- Create `ChurnStatus` to classify customers as `Churned` or `Active`.
- Remove the original `Churn` and `Complain` columns after creating the new attributes.

### 3. Customer Data Analysis

Use SQL queries to investigate:

- Active versus churned customer counts.
- Average tenure and total cashback of churned customers.
- Percentage of churned customers who complained.
- Churn patterns across city tiers and order categories.
- Preferred payment modes among active customers.
- Purchasing behavior based on marital status and ordering preferences.
- Coupon usage by gender.
- Customer satisfaction and complaint patterns.
- Order counts and average cashback across product categories.
- Customer distribution by warehouse-to-home distance.

### 4. Customer Returns Analysis

- Create a `customer_returns` table in the `ecomm` database.
- Insert the provided return records.
- Join return records with customer data.
- Retrieve return details for customers who have churned and submitted complaints.

## Key Learnings

- Applying SQL techniques to real-world business problems.
- Cleaning inconsistent data and handling missing values.
- Creating derived columns for meaningful analysis.
- Using aggregate functions, conditional filtering, and subqueries.
- Analyzing customer behavior through grouped queries.
- Combining multiple tables to investigate customer returns and churn.
- Translating customer data into insights that can support retention decisions.

## Conclusion

This project demonstrates the practical application of MySQL for customer churn analysis, from data cleaning and transformation to advanced querying and customer-return analysis. It strengthens SQL skills while connecting database analysis with real-world e-commerce business challenges.
