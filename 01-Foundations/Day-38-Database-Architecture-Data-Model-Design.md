# Day 38 – Database Architecture & Data Model Design

## Objective

Design the database architecture and data model for MoM Insight 360.

The goal is to create a scalable and reliable data foundation that supports Validation, Revenue, KPI, Forecast, and Executive Reporting Agents.

---

# Why Database Design Matters

AI Agents are only as effective as the data they consume.

A well-designed database:

- Improves performance
- Improves data quality
- Supports analytics
- Enables future scalability
- Reduces reporting complexity

---

# Database Architecture

Source Files
↓
Data Staging Layer
↓
Master Data Layer
↓
Transaction Data Layer
↓
Analytics Layer
↓
AI Agents
↓
Reports & Dashboards

---

# Database Layers

## 1. Staging Layer

Purpose:

Store raw uploaded files before validation.

Tables:

- Staging_Billing
- Staging_Scans
- Staging_Referrals

---

## 2. Master Data Layer

Purpose:

Store business master records.

Tables:

### Branch_Master

- Branch_ID
- Branch_Name
- Location
- Status

### Doctor_Master

- Doctor_ID
- Doctor_Name
- Specialty
- Branch_ID

### Referral_Master

- Referral_ID
- Referral_Name
- Referral_Type

### PRO_Master

- PRO_ID
- PRO_Name
- Branch_ID

---

## 3. Transaction Layer

Purpose:

Store operational business data.

### Billing_Fact

- Invoice_ID
- Invoice_Date
- Branch_ID
- Doctor_ID
- Revenue
- Scan_Count

### Scan_Fact

- Scan_ID
- Scan_Date
- Branch_ID
- Scan_Type
- Revenue

---

## 4. Analytics Layer

Purpose:

Store calculated business intelligence results.

### Revenue_Summary

- Date
- Branch
- Revenue
- Growth_Percentage

### KPI_Summary

- KPI_Name
- KPI_Value
- Target_Value
- Achievement_Percentage

### Forecast_Summary

- Forecast_Date
- Forecast_Type
- Forecast_Value

### Executive_Report_Summary

- Report_Date
- Key_Insights
- Risks
- Opportunities
- Recommendations

---

# Entity Relationships

Branch_Master
↓
Doctor_Master
↓
Billing_Fact

Branch_Master
↓
Scan_Fact

Referral_Master
↓
Billing_Fact

PRO_Master
↓
Billing_Fact

---

# Data Flow

Excel Upload
↓
Staging Tables
↓
Validation Agent
↓
Master Tables
↓
Transaction Tables
↓
Analytics Tables
↓
AI Agents
↓
Executive Reports

---

# Data Quality Considerations

- Primary Keys
- Foreign Keys
- Duplicate Prevention
- Data Validation Rules
- Audit Columns
- Error Logging

---

# Scalability Considerations

Future Support:

- Multiple Branches
- Multiple Hospitals
- Multiple Regions
- Additional AI Agents
- Power BI Integration
- Cloud Deployment

---

# Enterprise Perspective

The database serves as the central source of truth for MoM Insight 360.

Every AI Agent relies on accurate and well-structured data to generate reliable business intelligence.

---

# Key Takeaway

Strong AI systems are built on strong data foundations.

A well-designed database architecture ensures scalability, reliability, and trustworthy business insights.