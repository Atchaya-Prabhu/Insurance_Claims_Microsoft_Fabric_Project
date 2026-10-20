
# Insurance Claims KPI Analytics | Microsoft Fabric

## 📌 Project Overview

This project focuses on building an end-to-end insurance analytics platform using **Microsoft Fabric** and the **Medallion Architecture**.

A mid-sized insurance company provides Health, Auto, and Life Insurance policies. Customers regularly submit claims against their policies, but the company lacks a unified view of customer behavior, claims performance, policy risk, and approval trends.

The goal is to transform raw customer, policy, and claims data into clean, analytics-ready datasets that support insurance KPI analysis and business decision-making.

## 🏢 Business Problem

The company needs a unified view of:

- Customer behavior and claims patterns over time.
- Policy types generating the highest number of claims.
- Customers with high claim-to-coverage ratios.
- Gender-wise and demographic claim patterns.
- Claim approval and rejection trends across policy types.

## 🎯 Project Objectives

- Ingest customer, policy, and claims data into Microsoft Fabric.
- Clean, join, and aggregate data using the Medallion Architecture.
- Organize data into Bronze, Silver, and Gold layers.
- Combine Silver and Gold transformation logic to create a consolidated customer-level summary.
- Enable executives and analysts to explore KPIs and trends directly through Fabric notebooks without requiring Power BI.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Microsoft Fabric | End-to-end data engineering platform |
| Fabric Lakehouse | Store and organize datasets |
| OneLake | Unified data storage |
| PySpark | Data cleansing and transformation |
| Delta Lake | Reliable table storage |
| Fabric Notebooks | Data processing and analytics |
| Medallion Architecture | Structure data into Bronze, Silver, and Gold layers |

## 🏗️ Solution Architecture

### 🥉 Bronze Layer — Raw Data

- Ingest raw customer, policy, and claims datasets.
- Preserve source data for downstream processing.
- Store raw data in the Bronze Lakehouse layer.

### 🥈 Silver Layer — Cleaned and Transformed Data

- Handle missing and inconsistent values.
- Identify and remove duplicate records.
- Validate data types and business rules.
- Join customer, policy, and claims datasets.
- Standardize data for reliable downstream analysis.

### 🥇 Gold Layer — Business-Ready Data

- Aggregate claims data at customer and policy levels.
- Calculate insurance KPIs and performance metrics.
- Generate a consolidated customer-level summary.
- Prepare curated datasets for business analysis.

## 📊 Key Insurance KPIs

The project aims to analyze:

- Total claims and claims by insurance type.
- Claim approval and rejection rates.
- Claim amounts by policy type.
- Customer-level claim-to-coverage ratios.
- Demographic claim patterns.
- Claims trends over time.

## 🔄 Data Engineering Workflow

1. Ingest raw insurance datasets.
2. Store source data in the Bronze Lakehouse.
3. Clean and validate records in the Silver layer.
4. Join customer, policy, and claims data.
5. Aggregate data and calculate KPIs in the Gold layer.
6. Create a consolidated customer-level summary.
7. Analyze insurance KPIs using Fabric notebooks.

## 📁 Repository Structure

```text
insurance-claims-kpi-analytics/
│
├── README.md
├── data/
│   └── README.md
├── notebooks/
│   ├── 01_bronze_data_ingestion.ipynb
│   ├── 02_silver_data_transformation.ipynb
│   └── 03_gold_claims_analytics.ipynb
├── pipelines/
│   └── README.md
└── docs/
    └── architecture.md
```

## 🚀 Expected Outcome

The project will demonstrate how Microsoft Fabric can transform raw insurance data into reliable, analytics-ready datasets.

The resulting platform will provide a unified view of customer claims, policy performance, claim approval trends, and insurance KPIs to support data-driven decision-making.

## 💡 Skills Demonstrated

- Microsoft Fabric data engineering
- Medallion Lakehouse architecture
- PySpark and SQL transformations
- Delta Lake
- Data cleansing and validation
- Data integration and aggregation
- Data modeling and KPI analysis
- Insurance analytics
