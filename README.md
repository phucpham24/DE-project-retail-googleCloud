# Data Pipeline with Astro CLI, Cosmos, Airflow, Google Cloud, and BigQuery


## Overview

This repository contains a comprehensive Data Pipeline solution that leverages Astro CLI, Cosmos, Apache Airflow, Google Cloud services, and Docker. It enables the efficient extraction, transformation, and loading of data into BigQuery, making it a powerful tool for data processing and analysis.

## Key Components

The project incorporates the following key components:

1. **Astro CLI**: The Astro CLI is used to set up and manage the Airflow environment, allowing for the orchestration of data workflows and tasks. It provides a user-friendly interface for configuring and scheduling data pipelines.

2. **Cosmos**: Cosmos plays a vital role in data transformation and orchestration. It facilitates data cleansing, enrichment, and transformation tasks, enhancing data quality as it flows through the pipeline.

3. **Airflow**: Airflow serves as the core of the data pipeline, enabling the creation and execution of Directed Acyclic Graphs (DAGs) to manage data workflows. It is responsible for tasks such as data extraction, transformation, and loading (ETL).

4. **Google Cloud**: Google Cloud provides the infrastructure for data storage, offering Google Cloud Storage for raw and processed data. It ensures scalability, security, and reliability for data storage needs.

5. **BigQuery**: BigQuery is utilized for data analysis and querying. It allows for the storage and retrieval of processed data, supporting advanced analytics and reporting.
 
6. **Docker**: Containerization with Docker ensures portability and easy deployment of the pipeline across different environments.


## Project Structure

Explain the structure of your project, including directories, files, and their purposes.
```plaintext
.
├── airflow_settings.yaml
├── dags
│   └── retail.py
├── Dockerfile
├── include
│   ├── dataset
│   │   └── online_retail.csv
│   ├── dbt
│   │   ├── cosmos_config.py
│   │   ├── dbt_project.yml
│   │   ├── models
│   │   │   ├── report
│   │   │   │   ├── report_customer_invoices.sql
│   │   │   │   ├── report_product_invoices.sql
│   │   │   │   └── report_year_invoices.sql
│   │   │   ├── sources
│   │   │   │   └── sources.yml
│   │   │   └── transform
│   │   │       ├── dim_customer.sql
│   │   │       ├── dim_datetime.sql
│   │   │       ├── dim_product.sql
│   │   │       └── fct_invoices.sql
│   │   ├── packages.yml
│   │   └── profiles.yml
│   ├── gcp
│   │   └── service_account.json
│   └── soda
│       ├── check_function.py
│       ├── checks
│       │   ├── report
│       │   │   ├── report_customer_invoices.yml
│       │   │   ├── report_product_invoices.yml
│       │   │   └── report_year_invoices.yml
│       │   ├── sources
│       │   │   └── raw_invoices.yml
│       │   └── transform
│       │       ├── dim_customer.yml
│       │       ├── dim_datetime.yml
│       │       ├── dim_product.yml
│       │       └── fct_invoices.yml
│       └── configuration.yml
├── packages.txt
├── plugins
├── README.md
├── requirements.txt
├── structure.txt
└── tests
    └── docker-compose.override.yml
```
## Data Flow
<img width="1509" alt="Screenshot 2023-07-13 at 16 41 19" src="https://github.com/phucpham24/DE-project-retail-googleCloud/assets/118487319/bae9bab5-409b-4785-b324-556aee04c4a0">


## Relational Diagram
![EDR](https://github.com/phucpham24/DE-project-retail-googleCloud/assets/118487319/62bb41bc-cbfd-4d92-9ec6-9c4c4786d252)


## Data Visualization

Explain how to use Metabase to create data visualizations. Describe the process of creating dashboards, visualizations, and asking questions.

## Conclusion



