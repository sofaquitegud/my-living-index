# 🇲🇾 Malaysia Cost of Living & Salary Reality

An end-to-end data engineering project built on Databricks Free Edition
using public data from [data.gov.my](https://data.gov.my).

## Business Question
**Are Malaysians actually getting poorer?**

## Architecture
Bronze → Silver → Gold (Medallion Architecture)

## Data Sources (DOSM / data.gov.my)
- CPI Monthly & Annual
- Household Income (HIES)
- HIES by State
- Income Percentile Distribution
- Labour Force Statistics

## Key Findings
- Income beat inflation in 9 out of 10 survey periods (2002–2022)
- 2020 was the only year purchasing power declined (COVID impact)
- T20 earns 5.87x more than B40 as of 2024
- No state spends more than it earns at the median level

## Tech Stack
- Databricks
- Delta Lake (Bronze / Silver / Gold)
- PySpark
- Plotly + Matplotlib
- Lakeview Dashboard (AI/BI)

## Notebooks
| Notebook | Purpose |
|---|---|
| 00_setup_and_config | Create schemas, define config |
| 01_bronze_ingestion | Ingest 7 datasets from data.gov.my |
| 02_silver_transformation | Clean, type-cast, enrich |
| 03_gold_analytics | Build analytical Gold tables |
| 04_analysis_and_insights | Visualisations + final verdict |
