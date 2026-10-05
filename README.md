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
- ## Analysis Approach

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
