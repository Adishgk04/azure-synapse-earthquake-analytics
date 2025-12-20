## Earthquake Analytics Platform on Azure (USGS Data)

## Overview
This project implements an end-to-end **cloud data engineering and analytics solution** using **Azure Synapse Analytics**, **GitHub-based Continuous Integration**, and **Power BI**, analyzing **10+ years of global earthquake data** sourced from the USGS Web API.

The solution follows a **Medallion Architecture (Bronze → Silver → Gold)** to transform raw API data into business-ready analytical views, enabling insights into earthquake trends, severity, alerts, and regional risk.

---

## Architecture
- **Bronze Layer**: Raw JSON data ingested from the USGS Web API and stored in Azure Blob Storage
- **Silver Layer**: Cleaned and standardized earthquake dataset created using Synapse Data Flows
- **Gold Layer**: Aggregated analytical views built using Synapse Serverless SQL
- **CI Integration**: Azure Synapse workspace connected to GitHub for version control and collaboration
- **Visualization Layer**: Power BI reports connected via DirectQuery to Gold views

---

## Key Features
- REST API-based ingestion using Azure Synapse
- Medallion Architecture (Bronze / Silver / Gold)
- Serverless SQL analytics (cost-efficient, on-demand)
- GitHub-based Continuous Integration for Synapse artifacts
- Percentile-based classification for significant earthquake events
- Region, time-series, and alert-based aggregations
- Interactive Power BI dashboards

---

## Power BI Dashboards
1. Global Earthquake Overview & Temporal Trends  
2. Regional & City-Level Earthquake Impact Analysis  
3. Earthquake Risk, Alerts & Event Characteristics  

---

## Technology Stack
- Azure Synapse Analytics (Serverless SQL, Data Flows)
- Azure Blob Storage
- GitHub (Continuous Integration & version control)
- REST APIs (USGS)
- Power BI
- SQL, DAX

---

## Key Learnings
- Implementing CI with GitHub for Azure Synapse development
- Designing BI-ready Gold views from raw API data
- Handling large-scale, skewed datasets (~1.7M records)
- Applying real-world cloud data engineering best practices

---

## Future Enhancements
- Automated ingestion with scheduled triggers
