# Rockbuster SQL Business Analysis

### Customer, Market and Revenue Analysis Using SQL
## Executive Summary

This project uses SQL to analyse Rockbuster's customer, geographic and revenue data to support business decision-making.

The analysis moves from broad market-level questions to individual customer targeting, identifying:

- Countries with the largest customer bases
- Priority cities within key markets
- High-value customers for targeted rewards
- Revenue patterns that can support market prioritisation

The project demonstrates how SQL can be used not only to retrieve data, but to answer practical business questions and translate database information into actionable insights.
## Business Problem

Rockbuster Stealth is a fictional movie rental company planning how to compete in a changing entertainment market.

Management needed to better understand its existing customer and revenue data to determine where business activity was concentrated and which customers and markets should receive greater attention.

The analysis focuses on three practical questions:

1. Which countries and cities contain the largest customer bases?
2. Which customers generate the most revenue within priority markets?
3. How can these insights support targeted marketing and customer reward initiatives?
4. ## Tools & SQL Skills

- **SQL** — querying and analysing relational business data
- **INNER JOINs** — combining customer, address, city, country and payment data
- **GROUP BY & Aggregation** — calculating customer counts and revenue metrics
- **Subqueries** — answering multi-stage business questions
- **Common Table Expressions (CTEs)** — structuring more complex queries clearly
- **Filtering & Sorting** — identifying priority markets and customers
- **Business Analysis** — translating query results into commercial recommendations
- 
## Analysis Approach
## Key Findings

### 1. Customer Distribution Was Concentrated in Key International Markets
Geographic analysis identified a group of countries with comparatively large Rockbuster customer bases, providing a starting point for market prioritisation.

### 2. Revenue Analysis Refined the Geographic Picture
Customer volume alone did not provide the complete business picture. Using a CTE and payment data allowed cities within priority countries to be ranked by total revenue.

### 3. High-Value Customers Could Be Identified for Targeted Campaigns
By combining customer, payment and geographic data, the analysis identified the five highest-spending customers within priority cities.

These customers represent potential candidates for targeted rewards, retention initiatives or personalised marketing campaigns.

### 4. SQL Supported a Business Funnel from Market to Customer
The analysis progressively narrowed the decision from countries → cities → revenue → individual high-value customers, demonstrating how relational data can support increasingly targeted business decisions.
## Business Recommendations

Based on the analysis, Rockbuster could use its customer and revenue data to support several commercial decisions:

### 1. Prioritise Markets Using Both Customer Volume and Revenue
Avoid evaluating markets solely by customer numbers. Combine customer concentration with revenue performance when deciding where marketing resources should be focused.

### 2. Focus Marketing on High-Performing Cities
Cities generating strong revenue within priority countries can be used as starting points for more targeted regional campaigns.

### 3. Develop High-Value Customer Campaigns
Use customer-level spending data to identify high-value customers for personalised rewards, retention offers or loyalty initiatives.

### 4. Extend the Analysis Beyond Total Spend
Future analysis could incorporate rental frequency, customer tenure and recent activity to build a more complete picture of customer value and loyalty.

The analysis followed a funnel from broad geographic opportunity to individual customer targeting.

### 1. Geographic Market Profiling

The first stage identified the countries with the largest Rockbuster customer bases.

SQL joins connected the `customer`, `address`, `city` and `country` tables, while `COUNT`, `GROUP BY`, `ORDER BY` and `LIMIT` were used to rank markets by customer numbers.

### 2. Priority City Analysis

The analysis then narrowed the focus to cities within priority countries.

Filtering and grouping were used to identify urban markets where targeted business activity could have the greatest potential reach.

### 3. High-Value Customer Identification

Finally, customer and payment data were combined to identify high-value customers within target markets.

Revenue was aggregated at customer level using multi-table joins and `SUM`, allowing customers to be ranked by total spending for potential targeted rewards or marketing initiatives.
