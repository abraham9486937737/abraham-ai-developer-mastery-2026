# Day 26 – Data Cleaning for Agentic AI Systems

AI Developer Mastery 2026
Practical Project: AI-Commerce-Intelligence-Crew

# Day 26 – Data Cleaning for Agentic AI Systems

## Why Data Cleaning Matters

AI agents are only as good as the data they consume.

Even the most advanced LLM, CrewAI workflow, or Multi-Agent System will produce poor results if the underlying data is incomplete, inconsistent, duplicated, or incorrect.

Before building Sales Intelligence Agents, Customer Intelligence Agents, and Executive Reporting Agents, the dataset must be prepared and validated.

Data Cleaning is the bridge between Raw Data and Reliable Intelligence.

---

## Dataset Used

Project:
AI-Commerce-Intelligence-Crew

Dataset:
E-Commerce Sales Analytics Dataset

Primary File:
ecommerce_sales.csv

Rows:
138,116

Columns:
46

---

## Objectives

The objectives of Day 26 were:

- Identify missing values
- Identify duplicate records
- Validate data types
- Detect inconsistent values
- Standardize formats
- Prepare agent-ready datasets

---

## Data Quality Assessment

### Dataset Shape

Rows:
138,116

Columns:
46

### Data Types

- Object Columns
- Numeric Columns
- Boolean Columns
- Date Columns

Validated all fields.

---

## Missing Value Analysis

Important observations:

### delivery_days

Contains missing values.

### estimated_delivery_days

Contains missing values.

### return_status

Contains large number of null values.

### return_reason

Contains large number of null values.

### coupon_code

Contains many null values.

---

## Business Interpretation

Not every null value represents bad data.

Examples:

Return Status:
Null means order was never returned.

Return Reason:
Null means no return occurred.

Coupon Code:
Null means no coupon applied.

This is business logic rather than data quality issue.

---

## Duplicate Analysis

Checked:

order_id

Result:

No business duplicates found.

Dataset considered unique.

---

## Date Validation

Converted:

order_date

From:

Object

To:

Datetime

Benefits:

- Monthly analysis
- Quarterly analysis
- Seasonal analysis
- Trend analysis

---

## Standardization Activities

Validated:

- Order Status
- Payment Status
- Shipping Methods
- Sales Channels
- Customer Segments

No major inconsistencies found.

---

## Outlier Review

Reviewed:

- Revenue
- Profit
- Customer Lifetime Value

Extreme values retained because they represent actual business transactions.

---

## Agent Readiness Validation

Prepared dataset for:

### Sales Intelligence Agent

Revenue
Profit
Growth
Performance

### Customer Intelligence Agent

Customer Segments
Repeat Customers
CLV

### Product Intelligence Agent

Product Performance
Category Analysis

### Executive Reporting Agent

KPI Narratives
Business Summaries
Recommendations

---

## Key Learning

Data Cleaning is not about removing data.

It is about understanding business meaning behind the data.

Agentic AI requires clean, trusted, and business-ready datasets before intelligence can be generated.

---

## Day 26 Summary

Completed:

✓ Missing Value Analysis

✓ Duplicate Validation

✓ Data Type Validation

✓ Date Conversion

✓ Standardization Review

✓ Agent Readiness Assessment

Result:

Dataset is ready for Agent Development Phase.