# Day 35 – Validation Agent Design

## Objective

Design the Validation Intelligence Agent for MoM Insight 360.

The Validation Agent is responsible for ensuring data quality, accuracy, consistency, and reliability before data is consumed by Revenue, KPI, Forecast, and Executive Reporting Agents.

The goal is to prevent incorrect business insights caused by poor-quality data.

---

## Business Questions

1. Is the incoming data complete?
2. Are there missing values?
3. Are there duplicate records?
4. Are revenue values valid?
5. Are KPI calculations valid?
6. Does the data comply with business rules?
7. Are branch and doctor references valid?
8. Can the data be trusted for decision-making?

---

## Validation Categories

### Data Quality Validation

- Missing Values
- Null Values
- Blank Fields
- Invalid Data Types

### Duplicate Validation

- Duplicate Billing Records
- Duplicate Patients
- Duplicate Referrals

### Revenue Validation

- Negative Revenue Check
- Revenue Mismatch Check
- Invalid Billing Amounts

### KPI Validation

- KPI Formula Validation
- Target Validation
- Percentage Validation

### Master Data Validation

- Branch Validation
- Doctor Validation
- Referral Validation
- PRO Validation

### Business Rule Validation

- Revenue cannot be negative
- Scan count cannot be negative
- Referral count cannot be negative
- Invoice date cannot be in the future
- Branch must exist in master data
- Doctor must exist in master data

---

## Validation Outputs

### Validation Summary

- Records Processed
- Passed Records
- Warning Records
- Error Records
- Data Quality Score

### Exception Report

PASS
WARNING
ERROR

### Recommendations

- Missing Data Corrections
- Duplicate Removal
- Master Data Updates
- Revenue Validation Actions

---

## Validation Workflow

Raw Data
↓
Data Quality Checks
↓
Duplicate Checks
↓
Revenue Validation
↓
KPI Validation
↓
Business Rule Validation
↓
Exception Detection
↓
Validation Report
↓
Trusted Data

---

## Example Output

Records Processed : 25,430

Passed Records : 25,100

Warnings : 280

Errors : 50

Data Quality Score : 98.7%

---

## Enterprise Perspective

The Validation Agent is the foundation of MoM Insight 360.

Without validated data, Revenue, KPI, Forecasting, and Executive Reporting cannot be trusted.

The Validation Agent ensures that all downstream agents work with reliable business data.

---

## Key Takeaway

Trusted insights start with trusted data.

The Validation Agent acts as the quality gatekeeper for the entire MoM Insight 360 platform.