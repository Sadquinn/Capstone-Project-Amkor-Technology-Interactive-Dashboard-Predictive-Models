# Capstone Project – Amkor Technology Interactive Dashboard & Predictive Models

## Project Overview

This capstone project delivers an end-to-end analytics and forecasting solution for Amkor Technology, combining an interactive Power BI dashboard with two predictive models to support strategic decision-making. The project addresses the challenge of fragmented financial and operational data by consolidating multiple external and internal sources into a unified, automated, and insight-driven platform.

The solution consists of two core components:
1. An interactive Power BI dashboard for real-time performance monitoring and competitive benchmarking  
2. Predictive models to forecast **ROIC–WACC spread** and **Revenue**

---

## Executive Summary

Amkor Technology’s decision-makers face limited real-time visibility into customer, vendor, and competitor performance due to data being scattered across SEC filings, Bloomberg Terminal, and analyst reports. This fragmentation results in manual, time-consuming analysis and weak predictive capabilities.

This project resolves these challenges by delivering an interactive Power BI dashboard that integrates customer and competitor KPIs into a single analytics environment. Automated data pipelines built with Excel Power Query and VBA macros consolidate data from multiple sources, significantly reducing manual preparation effort. The dashboard provides comprehensive visibility into revenue trends, profitability, operational efficiency, and competitive positioning, enabling Finance, Investor Relations, and Inventory Management teams to move from reactive reporting to proactive, data-driven decision-making.

In addition, predictive models are developed to forecast future **ROIC–WACC spread** and **Revenue**, enhancing Amkor’s ability to anticipate financial performance and support long-term strategic planning.

---

## Project Objectives

- **Centralize Data Integration**  
  Consolidate customer, vendor, and competitor data from SEC filings, Bloomberg Terminal, and analyst reports into a single Power BI dashboard.

- **Automate Data Processing**  
  Replace manual data preparation with automated pipelines using Excel Power Query and VBA macros, reducing preparation time by approximately 70%.

- **Enable Actionable Insights**  
  Provide interactive, real-time visualizations covering revenue performance, profitability, operational efficiency, and market positioning.

- **Establish Competitive Benchmarking**  
  Systematically compare Amkor’s performance against key competitors: ASE Technology (ASE), Powertech Technology Inc. (PTI), and Jiangsu Changjiang Electronics Technology (JCET).

- **Support Strategic Decision-Making**  
  Shift reporting from historical review to forward-looking, predictive analytics for Finance, Investor Relations, and Inventory Management teams.

---

## Project Scope

- **Dashboard Development**  
  Interactive Power BI dashboard with automated data pipelines (Excel Power Query, VBA), integrating Bloomberg Terminal data, SEC filings, and analyst reports from 2021–2025.

- **Competitive Analysis**  
  Benchmarking framework comparing Amkor with ASE (primary competitor), PTI, and JCET across financial, operational, and market metrics.

- **Predictive Modeling**  
  Two forecasting models developed to predict:
  - ROIC–WACC spread  
  - Revenue

- **Stakeholder Deployment**  
  Enablement for Finance, Investor Relations, and Inventory Management through documentation and user guidance.

---

## Key Metrics and KPIs

The dashboard tracks critical metrics across five analytical dimensions:

### Financial Performance
- Revenue Growth YoY (%)
- Total Revenue (Quarterly and Annual)
- Revenue by Segment
- Revenue by Region (Asia, Americas, EMEA)
- Packaging & Testing Revenue Growth YoY

### Profitability Metrics
- Earnings Per Share (Adjusted Diluted)
- Gross Margin (%)
- Net Margin (%)
- Total Net Income

### Efficiency Ratios
- Asset Turnover
- Revenue per Property, Plant & Equipment (PPE)
- Inventory Turnover

### Operational Efficiency
- Market Share (%) by Company
- Market Share (%) – Packaging & Testing Segment
- R&D Expense Ratio to Revenue

### Customer Metrics
- Top Revenue-Contributing Customers
- Competitor Landscape for Key Customers

---

## System Architecture

### Data Sources
- **Bloomberg Terminal**: Financial metrics for Amkor, ASE, JCET, and PTI  
- **SEC Filings (10-K, 10-Q)**: Financial statements, revenue segments, customer concentration, CAPEX, and R&D  
- **Company Investor Relations**: Presentations and press releases  

### Technology Stack
- Adobe PDF  
- Microsoft Excel  
- VBA Macros  
- Power Query  
- Power BI  
- DAX  

---

## Technical Implementation

### Data Extraction and Preparation

#### Bloomberg Terminal Data Extraction
- Retrieve financial data for AMKR, ASE, JCET, and PTI via Bloomberg Terminal
- Download datasets in PDF format
- Convert PDFs to Excel
- Clean and standardize data structure
- Consolidate values into a unified Power BI staging table

#### Power Query Transformation
- Reshape data into a normalized schema:
  
  `Company | Metric | Date | Value`

- Standardize metric definitions using Amkor as the baseline taxonomy
- Harmonize naming conventions across all competitors

---

## VBA Automation for Regional Segmentation

### Business Problem
Bloomberg’s segment-by-region data is formatted in wide, crosstab layouts unsuitable for Power BI, requiring hours of manual reshaping per company and quarter.

### Automation Solution
A custom VBA macro (`Flatten_SegmentByRegion`) automatically converts crosstab data into a normalized, Power BI–ready format:

`Company | Date | Metric | Region | Value`

### Performance Impact
- Manual Processing: 2–3 hours per company  
- Automated Processing: <5 seconds  
- Time Savings: ~95% reduction  
- Error Rate: Reduced from ~15% to <1%

---

## Data Quality Assurance

- Spot-check validation of random data points
- Completeness checks based on expected row counts
- Removal of aggregate “Total” rows to prevent double-counting
- Power BI integration testing for relationships and measure accuracy

---

## User Guide

The Power BI file will be shared along with all supporting Excel data sources after project completion. To use the dashboard:

1. Download the Power BI file and associated Excel files
2. Open the Power BI file locally
3. Refresh the data to load the latest metrics and visualizations

---
