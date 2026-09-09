# 🛒 Walmart Data Engineering Project

An end-to-end data engineering pipeline built to demonstrate **CDC ingestion, distributed processing, data transformation, orchestration, and analytics-ready data modeling**.

## 🏗️ Architecture

**Ghost Agentic DB**  
↓  
**CDC / Incremental Ingestion**  
↓  
**Databricks + Apache Spark**  
↓  
**Bronze Layer**  
↓  
**dbt Transformations**  
↓  
**Silver Layer**  
↓  
**dbt Transformations**  
↓  
**Gold Layer — Facts & Dimensions**

**AWS S3** is used as cloud storage / data lake.

**Apache Airflow** orchestrates the pipeline.

---

## ⚙️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Databricks** | Data engineering & processing |
| **Apache Spark** | Distributed data processing |
| **dbt** | SQL transformations, testing & snapshots |
| **Apache Airflow** | Pipeline orchestration |
| **Ghost Agentic DB** | Source database |
| **AWS S3** | Cloud storage / data lake |
| **Docker** | Containerized environment |
| **Python** | Pipeline development |
| **SQL** | Data transformation |
| **Git & GitHub** | Version control |

---

## 🔄 Pipeline

**Source → Ingestion → Bronze → Silver → Gold**

- **Bronze** — Raw ingested data
- **Silver** — Cleaned and transformed data
- **Gold** — Analytics-ready facts and dimensions

---

## 🚀 Key Features

- CDC / incremental data ingestion
- Databricks & Spark processing
- Medallion architecture
- dbt transformations and data quality tests
- dbt snapshots for historical tracking
- Airflow pipeline orchestration
- AWS S3 cloud storage
- Dockerized development environment

---

## 📂 Project Structure

```text
airflow_dbt_project/
│
├── airflow/
│   ├── dags/
│   ├── config/
│   ├── docker-compose.yaml
│   ├── Dockerfile
│   └── requirements.txt
│
└── walmart_project/
    ├── models/
    │   ├── source/
    │   ├── silver_t/
    │   ├── silver_b/
    │   └── gold/
    ├── snapshots/
    ├── tests/
    ├── macros/
    ├── dbt_project.yml
    └── profiles.yml
👨‍💻 Author

Akshat Jain

Data Engineering • Databricks • dbt • Airflow • Python • SQL
