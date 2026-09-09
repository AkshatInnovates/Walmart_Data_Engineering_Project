# Walmart Data Engineering Project

An end-to-end data engineering project demonstrating a modern ELT pipeline using **Ghost Agentic Database, Databricks, Apache Spark, dbt, Apache Airflow, Docker, AWS S3, Python, and SQL.**

## Architecture

```text
Ghost Agentic DB
       │
       │ CDC / Incremental Data
       ▼
  Databricks
       │
    Spark
       │
       ▼
  Bronze Layer
       │
      dbt
       ▼
  Silver Layer
       │
      dbt
       ▼
   Gold Layer
 Facts + Dimensions

AWS S3
   │
   └── Cloud Storage / Data Lake
# Medallion Architecture
Bronze → Raw ingested data
Silver → Technical + business transformations
Gold → Facts and dimensions for analytics
# Tech Stack
Databricks & Apache Spark — Data processing
dbt — SQL transformations, testing & snapshots
Apache Airflow — Pipeline orchestration
Ghost Agentic Database — Source database
AWS S3 — Cloud storage / data lake
Docker — Containerized Airflow environment
Python & SQL — Development and transformations
Git & GitHub — Version control
# Pipeline
Source DB
   ↓
CDC / Incremental Ingestion
   ↓
Databricks + Spark
   ↓
Bronze
   ↓
dbt
   ↓
Silver
   ↓
dbt
   ↓
Gold
# Key Features
End-to-end data pipeline
CDC / incremental data processing
Medallion architecture
dbt transformations and data quality tests
dbt snapshots for historical tracking
Airflow orchestration
Databricks + Spark processing
AWS S3 cloud storage
Dockerized development environment
Author

Akshat Jain

Data Engineering | Databricks | dbt | Airflow | Python | SQL
