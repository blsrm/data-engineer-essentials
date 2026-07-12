## Full Mind Map - Data Engineering

```
                         DATA ENGINEERING
                                |
   ------------------------------------------------------------------
   |                |                |               |               |
BIG DATA        SPARK           DATABRICKS      CLOUD PLATFORMS   INGESTION
   |                |                |               |               |
Hadoop           Core Engine      Workspace       AWS / Azure / GCP Batch / Stream
HDFS             RDD / DF         DBFS            EMR / ADF / DP   Sqoop / Kafka
MapReduce        SQL / MLlib      Delta Lake      BigQuery / S3    CDC / ETL / ELT
Cloudera         Streaming        Auto Loader     Synapse / Glue   Incremental Loads

```

```
DATA ENGINEERING
│
├── BIG DATA FOUNDATIONS
│   ├── Hadoop
│   │   ├── HDFS (Storage)
│   │   ├── MapReduce (Processing)
│   │   └── YARN (Resource Manager)
│   ├── Cloudera (Enterprise Hadoop)
│   └── Concepts
│       ├── Distributed Storage
│       ├── Distributed Compute
│       └── Fault Tolerance
│
├── FILE FORMATS
│   ├── Parquet (Columnar)
│   ├── ORC
│   ├── Avro
│   └── JSON/CSV
│
├── DATA INGESTION
│   ├── Batch
│   │   ├── Sqoop
│   │   ├── ETL
│   │   └── ELT
│   ├── Streaming
│   │   ├── Kafka
│   │   ├── Kinesis
│   │   └── Pub/Sub
│   └── CDC (Change Data Capture)
│
├── CLOUD BIG DATA SERVICES
│   ├── AWS
│   │   ├── EMR
│   │   ├── Glue
│   │   ├── S3
│   │   └── Redshift
│   ├── Azure
│   │   ├── ADLS
│   │   ├── ADF
│   │   ├── Synapse
│   │   └── Azure Databricks
│   └── GCP
│       ├── DataProc
│       ├── DataFlow
│       ├── BigQuery
│       └── GCS
│
├── SPARK ECOSYSTEM
│   ├── Apache Spark
│   │   ├── RDD
│   │   ├── DataFrame
│   │   ├── SQL
│   │   ├── Streaming
│   │   └── MLlib
│   ├── PySpark
│   ├── Spark Cluster
│   │   ├── Master Node
│   │   └── Worker Nodes
│   └── Serialization
│
├── DATABRICKS PLATFORM
│   ├── Workspace
│   │   ├── Notebooks
│   │   ├── Repos
│   │   └── DBFS
│   ├── Delta Lake
│   │   ├── Delta Tables
│   │   ├── ACID
│   │   ├── Time Travel
│   │   └── Auto Loader
│   ├── Jobs & Workflows
│   └── MLflow
│
├── DATA WAREHOUSING
│   ├── SQL Warehouse
│   ├── Star Schema
│   ├── Snowflake Schema
│   ├── Fact Tables
│   └── Dimension Tables
│
└── DATA ENGINEER TOOLKIT
    ├── Git
    ├── Docker
    ├── Airflow
    ├── Terraform
    ├── Power BI / Tableau
    └── Python (Pandas, NumPy)

```

## Core Big Data Concepts
### Big Data
Large amounts of data that cannot be processed on one computer. Needs distributed systems.

### Hadoop
An open‑source framework to store and process big data across many machines.

### HDFS (Hadoop Distributed File System)
Storage layer of Hadoop.
Stores huge files by splitting them into blocks and distributing across machines.

### MapReduce
Processing layer of Hadoop.
Breaks a job into:
  Map → split work
  Reduce → combine results

### Cloudera
A company that provides enterprise Hadoop distributions and tools.

## SQL & Warehousing
### SQL
Language to query and manipulate data in databases.

### Warehouse / SQL Warehouse
A system optimized for analytics (not transactions).
Stores structured data and runs fast SQL queries.

### ACID
Database properties:

Atomic
Consistent
Isolated
Durable
Ensures reliable transactions.

### CDC (Change Data Capture)
Technique to capture only changed data (inserts/updates/deletes).

### Incremental Loads
Loading only new or changed data instead of full data every time.

## Data Movement Tools
### Sqoop
Tool to transfer data between Hadoop and relational databases.

### Sqoop Job
A saved Sqoop command that runs repeatedly (scheduled import/export).

### Data Proc
Google Cloud’s managed Hadoop/Spark service.

### Data Stream
Google Cloud’s streaming ingestion service (similar to Kafka).

## Spark Ecosystem
Spark
Fast, distributed data processing engine (much faster than Hadoop MapReduce).

### Apache Spark
The open-source version of Spark.

### Spark Cluster
Group of machines running Spark.

### Master Node
Controls the cluster, assigns tasks.

### Worker Nodes
Execute the tasks.

### PySpark
Python API for Spark.

### RDD (Resilient Distributed Dataset)
Low-level Spark data structure.
Requires manual optimization.

### DataFrame
High-level table-like structure.
Optimized automatically (recommended).

### RDD vs DataFrame (simple):  
RDD = manual, slow
DataFrame = optimized, fast


## Databricks Ecosystem
### Databricks
Cloud platform built on Spark with extra features for data engineering, ML, and collaboration.

### Notebooks
Interactive coding environment (Python, SQL, Scala).

### Jobs
Scheduled or automated tasks (ETL pipelines, scripts).

### Workflows
Chained jobs with dependencies (like Airflow).

### DBFS (Databricks File System)
Databricks’ internal storage layer.

### Delta Lake
Storage format built on top of Parquet with ACID transactions.

### Delta Table
A table stored in Delta format.

### Auto Loader
Databricks feature to automatically ingest new files from cloud storage.

### MLflow
Tool for tracking machine learning experiments, models, and deployments.



## Cloud Big Data Platforms
### BigQuery
Google Cloud’s serverless data warehouse.

### EMR (Elastic MapReduce)
AWS’s managed Hadoop/Spark service.


## File Formats
### Parquet
Columnar file format.
Fast for analytics, compresses well.

### Serializable
Ability to convert an object into a format that can be stored or transferred.

### ETL vs ELT
ETL (Extract → Transform → Load)
Transform data before loading into warehouse.

ELT (Extract → Load → Transform)
Load raw data first, then transform inside warehouse.


## Difference Between Databricks on Azure, AWS, GCP, Community Edition
### Azure Databricks
Deep integration with Azure services (ADLS, ADF, Azure SQL)

Best for enterprise security (AAD, VNET)

### AWS Databricks
Integrates with S3, Glue, Redshift

More flexibility for custom networking

### GCP Databricks
Integrates with GCS, BigQuery

Newer compared to Azure/AWS

### Community Edition
Free, limited version

Single small cluster

Good for learning, not for production


## Other Tools Used by Data Engineers
### Storage
AWS S3

Azure ADLS

GCP GCS

### Streaming
Kafka

Kinesis

Pub/Sub

### Orchestration
Airflow

Azure Data Factory

AWS Glue

Prefect

### Databases
MySQL

PostgreSQL

MongoDB

Cassandra

### Visualization
Power BI

Tableau

Looker

### DevOps
Git

Docker

Kubernetes

### ML Tools
TensorFlow

PyTorch

Scikit-learn





