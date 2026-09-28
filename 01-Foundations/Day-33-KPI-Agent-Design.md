# Day 33 – KPI Agent Design

## Objective

Design the KPI Intelligence Agent for MoM Insight 360.

The KPI Agent analyzes operational and business KPIs and provides insights, trends, exceptions, and recommendations.

---

## Business Questions

1. Are branch KPIs meeting targets?
2. Which branch performs best?
3. Which doctor contributes most?
4. Which referral sources generate maximum revenue?
5. Which PROs are performing well?
6. Which scan categories perform best?
7. What operational risks exist?
8. Which KPIs require management attention?

---

## Inputs

- Billing Data
- Referral Data
- Doctor Data
- Scan Data
- PRO Data
- Branch Data
- KPI Targets

---

## Outputs

- KPI Summary
- KPI Exceptions
- KPI Trends
- Top Performers
- Underperforming Areas
- Recommendations

---

## KPI Categories

### Revenue KPIs

- Revenue
- Revenue Growth %
- Revenue Variance

### Doctor KPIs

- Doctor Revenue
- Doctor Contribution %

### Referral KPIs

- Referral Revenue
- Referral Conversion %

### Scan KPIs

- Scan Volume
- Scan Revenue

### PRO KPIs

- Leads Generated
- Conversion %

### Branch KPIs

- Revenue by Branch
- Growth by Branch

---

## Workflow

Data
↓
KPI Calculation
↓
KPI Comparison
↓
Exception Detection
↓
Trend Analysis
↓
Recommendations
↓
Executive Summary

---

## Expected Output Example

Branch: Sahakarnagar

Revenue Target: ₹50 Lakhs
Actual Revenue: ₹47 Lakhs
Variance: -₹3 Lakhs

Observation:
Revenue below target by 6%.

Recommendation:
Increase referral engagement and scan conversion activities.