# Databricks End-to-End Medallion Architecture Project

This repository contains an end-to-end implementation of the **Medallion Architecture** (Bronze → Silver → Gold) using Databricks notebooks.  
The project demonstrates how to design scalable data pipelines for both **dimension** and **fact tables** in an e-commerce domain.

---

## 📂 Project Structure
- **1_medallion_processing_dim/**
  - `1_dim_bronze.ipynb` → Ingest raw dimension data into the Bronze layer
  - `2_dim_silver.ipynb` → Clean and transform dimension data into the Silver layer
  - `3_dim_gold.ipynb` → Curate dimension data for analytics in the Gold layer

- **2_Setup/**
  - `New Notebook ...` → Setup and configuration scripts

- **3_medallion_processing_fact/**
  - `1_fact_bronze.ipynb` → Ingest raw fact data into the Bronze layer
  - `2_fact_silver.ipynb` → Transform fact data into the Silver layer
  - `3_fact_gold.ipynb` → Curate fact data for reporting in the Gold layer

---

## 🏗️ Architecture Overview
The **Medallion Architecture** organizes data into three layers:
- **Bronze** → Raw, ingested data (minimal transformations)
- **Silver** → Cleaned, structured, and enriched data
- **Gold** → Aggregated, business-ready data for analytics and reporting

This layered approach improves **data quality, scalability, and reusability** across pipelines.

---

## ⚙️ Technologies Used
- **Databricks** (Free Edition)
- **Apache Spark** for distributed processing
- **Delta Lake** for ACID transactions and schema enforcement
- **GitHub** for version control

---

## 🚀 Getting Started
1. Clone the repository:
   ```bash
   git clone https://github.com/P1lat001/Databricks_end_to_end_Medallion_architecture_project_001.git
