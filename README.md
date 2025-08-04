# E-Commerce-Data-Pipeline (still working on it)
A complete data engineering and warehousing solution developed as a graduation project at the Information Technology Institute (ITI).  
The project demonstrates modern data engineering practices by combining batch and streaming pipelines to process and analyze transactional and user activity data.

Business Objective

The goal of this project is to enable data-driven decision-making by transforming raw sales and user activity data into clean, modeled datasets ready for analysis.  
We analyzed batch data to track sales performance, customer behavior, delivery trends, and seller activity, while also building a streaming layer for real-time user events (clicks, views, purchases, etc.) to support operational monitoring and alerting.

---

## 📁 Data Sources

- **Batch Data:** Collected from public APIs representing sales, customers, products, payments, reviews, and geolocation, simulating ERP and CRM systems.
- **Streaming Data:** Simulated in real-time using Python's Faker and served via FastAPI to represent user activity events (e.g. views, clicks, sessions).

---

## ⚙️ Architecture Overview

### 🛠 Batch Pipeline:
- Ingest data from API into HDFS  
- Process and clean data using Apache Spark  
- Load processed data into PostgreSQL  
- Transform and model using `dbt` (Star Schema)  
- Visualize using Power BI

### ⚡ Streaming Pipeline:
- Generate real-time user logs with Faker + FastAPI  
- Send data to Kafka topics  
- Consume and process with Spark Structured Streaming  
- Store data in HDFS and PostgreSQL  
- Monitor stream via Streamlit/Grafana

---

## 🧰 Tools & Technologies

- **Ingestion & Streaming:** Kafka, FastAPI, Faker  
- **Processing:** Apache Spark (Batch & Structured Streaming)  
- **Storage:** HDFS, PostgreSQL (Data Warehouse), Parquet  
- **Modeling:** dbt (Data Build Tool), Star Schema  
- **Orchestration:** Apache Airflow  
- **Visualization:** Power BI, Streamlit / Grafana  
- **Infrastructure:** Docker, Docker Compose  
- **Monitoring:** Email Notifications (SMTP), Streamlit Dashboards  

---

