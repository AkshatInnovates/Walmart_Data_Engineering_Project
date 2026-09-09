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

Author

Akshat Jain

Data Engineering | Databricks | dbt | Airflow | Python | SQL
