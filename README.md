# Customer Shopping Behavior Analysis

## Overview

Analyzing customer shopping behavior using transactional data from 3,900 purchases across various product categories. The objective is to uncover insights into customer demographics, spending behavior, product preferences, loyalty patterns, and subscription trends to guide strategic business decisions.

---

## Business Problem

A retail company wants to better understand its customers’ shopping behavior in order to improve sales, customer satisfaction, and long-term loyalty. The management team has noticed changes in purchasing patterns across demographics, product categories, and sales channels (online vs. offline). They are particularly interested in uncovering which factors, such as discounts, reviews, seasons, or payment preferences, drive consumer decisions and repeat purchases.

---

## Tools and Technologies

- Jupyter Notebook (VS Code)
- Python (Pandas)
- SQL (PostgreSQL)
- Power BI

---

## Project Structure

```bash
Customer-Shopping-Behavior-Analysis
│
├── customer_shopping_behavior.csv
├── project.ipynb
├── customer_behavior_analysis.sql 
├── customer_behavior_dashboard.pbix
└── requirements.txt
```

---

### Data Cleaning & Preparation
- Removed duplicate records
- Handled missing values in Review Rating
- Standardized categorical columns
- Verified data consistency and formatting
- Converted columns into appropriate datatypes

### Exploratory Data Analysis (EDA)

#### Performed analysis to identify:

- Customer purchasing behavior
- Product category trends
- Seasonal shopping patterns
- Subscription-based purchase trends
- Impact of discounts and promo codes
- Customer demographics insights

---

## How to run this Project Workflow 

### 1. Import Required Libraries

```python
import pandas as pd
import psycopg2
from sqlalchemy import create_engine
```

### 2. Load Dataset

```python
df = pd.read_csv('customer_shopping_behavior.csv')
```

### 3. Load Data into PostgreSQL Database

```python
engine_psql = create_engine("postgresql+psycopg2://postgres:password@localhost:5432/customer_behavior")
```

### 4. SQL Analysis & Business Queries

#### Executed SQL queries to analyze:

- Top-performing product categories
- Repeat customer behavior
- Subscription trends
- Seasonal sales performance
- Discount effectiveness
- Customer loyalty patterns

### 5. Connect Dataset to Power BI
```powerbi
dashboard/customer_behavior_dashboard.pbix
```

---

## Business Impact

### Key Insights

- Customers using subscriptions showed higher repeat purchase behavior
- Seasonal demand significantly influenced product category sales
- Discounts and promo codes positively impacted purchase frequency
- Certain demographics contributed more to high-value purchases
- Review ratings influenced customer retention and repeat orders

---

## Recommendations

- Personalize promotional campaigns based on customer segments
- Increase focus on high-performing seasonal categories
- Improve loyalty programs for repeat customers
- Use review ratings to improve product quality and customer satisfaction
- Optimize discount strategies to maximize profitability
