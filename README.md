# Data Engineering Notes

A collection of my notes, examples, and practical learnings about **Data Engineering**.

This repository is a personal knowledge base where I document concepts, tools, and approaches I learn while building data systems.

---

## What is Data Engineering?

Data Engineering is about building systems that collect, process, store, and deliver data so it can be used reliably for analytics, applications, and decision-making.

A typical data flow looks like:

```text
Data Sources
     ↓
Data Ingestion
     ↓
Data Storage
     ↓
Data Transformation
     ↓
Data Warehouse
     ↓
Analytics
```

Modern data engineering also focuses on:

* Data quality
* Reliability
* Scalability
* Security
* Monitoring
* Cost
* Maintainability

---

# 📚 Topics

## 1. Data Engineering Fundamentals

Understanding the basic concepts behind data engineering.

Topics:

* What is Data Engineering?
* Data pipelines
* ETL vs ELT
* Batch processing
* Stream processing
* Data ingestion
* Data transformation
* Data lakes
* Data warehouses
* Data lakehouses
* Structured vs unstructured data
* Schema and schema evolution
* Data quality
* Data lineage
* Metadata

---

## 2. SQL

SQL is one of the most important skills for working with data.

Topics:

* SQL fundamentals
* SELECT and WHERE
* GROUP BY and HAVING
* JOINs
* Subqueries
* CTEs
* CASE statements
* Aggregations
* Window functions
* Date and time operations
* NULL handling
* Set operations
* Query optimization

Examples and exercises are included where useful.

---

## 3. Python

Python is used for data ingestion, transformation, automation, APIs, and building pipelines.

Topics:

* Python fundamentals
* Variables and data types
* Lists, dictionaries, sets, tuples
* Functions
* Modules and packages
* File handling
* JSON
* APIs
* Exception handling
* Logging
* Virtual environments
* Pandas
* Testing
* Writing maintainable Python

---

## 4. Databases

Understanding how databases store and retrieve data.

Topics:

* Relational databases
* PostgreSQL
* Tables and relationships
* Primary keys
* Foreign keys
* Constraints
* Normalization
* Denormalization
* Indexes
* Transactions
* ACID
* Isolation levels
* Query execution
* Database performance

---

## 5. Data Storage

Understanding how data is stored in modern data platforms.

Topics:

* Object storage
* Data lakes
* Data warehouses
* Data lakehouses
* CSV
* JSON
* Parquet
* Avro
* Partitioning
* Compression
* File organization
* Storage optimization

---

## 6. Data Modeling

Designing data structures that are useful for analytics and applications.

Topics:

* Data modeling fundamentals
* OLTP vs OLAP
* Fact tables
* Dimension tables
* Grain
* Primary and surrogate keys
* Star schema
* Snowflake schema
* Dimensional modeling
* Slowly Changing Dimensions
* Data marts
* Semantic layers

---

## 7. Data Transformation

Turning raw data into clean and useful data.

Topics:

* ETL
* ELT
* SQL transformations
* Python transformations
* dbt
* Staging models
* Intermediate models
* Fact and dimension models
* Incremental models
* Data tests
* Documentation
* Transformation best practices

---

## 8. Data Orchestration

Managing and scheduling data pipelines.

### Apache Airflow

Topics:

* DAGs
* Tasks
* Operators
* Dependencies
* Scheduling
* Retries
* Backfills
* Sensors
* Connections
* Variables
* Monitoring
* Error handling
* Pipeline design

The main goal is to understand how to build **reliable and maintainable workflows**.

---

## 9. Distributed Data Processing

Processing large amounts of data across multiple machines.

### Apache Spark

Topics:

* Spark architecture
* Driver and executors
* DataFrames
* Spark SQL
* Transformations
* Actions
* Lazy evaluation
* Partitions
* Shuffles
* Joins
* Caching
* Broadcast joins
* Performance optimization
* PySpark

---

## 10. Data Streaming

Working with continuously generated data.

### Apache Kafka

Topics:

* Kafka architecture
* Brokers
* Topics
* Partitions
* Producers
* Consumers
* Consumer groups
* Offsets
* Replication
* Message delivery
* Event-driven architecture
* Stream processing

The focus is on understanding how real-time data pipelines work.

---

## 11. Cloud Data Engineering

Learning how modern data platforms are built in the cloud.

### AWS

Topics may include:

* S3
* IAM
* Glue
* Athena
* Redshift
* RDS
* Lambda
* CloudWatch

### Azure

Topics may include:

* Azure Data Lake Storage
* Azure Data Factory
* Azure Synapse
* Azure Databricks

### GCP

Topics may include:

* Cloud Storage
* BigQuery
* Dataflow
* Dataproc
* Pub/Sub

The focus is on **cloud data engineering concepts**, not simply learning individual services.

---

## 12. Data Quality

A data pipeline is only useful if the data can be trusted.

Topics:

* Data validation
* Completeness
* Accuracy
* Consistency
* Uniqueness
* Freshness
* Schema validation
* Data tests
* Data contracts
* Data lineage
* Monitoring
* Alerting
* Data observability

---

## 13. Infrastructure

Understanding how data infrastructure is created and managed.

Topics:

* Docker
* Terraform
* Infrastructure as Code
* CI/CD
* Environment management
* Secrets management
* Deployment
* Cloud infrastructure

---

## 14. Data Architecture

Understanding how different components work together to form a data platform.

Topics:

* Data platform architecture
* Data lake architecture
* Data warehouse architecture
* Lakehouse architecture
* Batch architecture
* Streaming architecture
* Distributed systems
* Scalability
* Reliability
* Security
* Cost optimization

---

#  Repository Structure

```text
data-engineering-notes/
│
├── 01-data-fundamentals/
│
├── 02-sql/
│
├── 03-python/
│
├── 04-databases/
│
├── 05-data-storage/
│
├── 06-data-modeling/
│
├── 07-data-transformation/
│
├── 08-orchestration/
│
├── 09-distributed-processing/
│
├── 10-streaming/
│
├── 11-cloud/
│
├── 12-data-quality/
│
├── 13-infrastructure/
│
└── 14-data-architecture/
```

Each folder contains notes and examples related to that topic.

---

#  Main Technologies

The technologies I plan to explore include:

```text
Languages
├── SQL
└── Python

Databases
└── PostgreSQL

Transformation
└── dbt

Orchestration
└── Apache Airflow

Processing
└── Apache Spark

Streaming
└── Apache Kafka

Cloud
├── AWS
├── Azure
└── GCP

Infrastructure
├── Docker
└── Terraform
```

This list will change as I learn and build more.

---

#  How I Take Notes

For each topic, I try to answer a few simple questions:

### What is it?

A simple explanation of the concept.

### Why do we use it?

The problem it solves.

### How does it work?

The important technical details.

### When should we use it?

Real-world use cases.

### What are the trade-offs?

Advantages, limitations, performance, and cost considerations.

### Example

A practical SQL, Python, architecture, or configuration example.

### Production Considerations

Things that matter when using the technology in a real data platform.

---

#  Practical Learning

I don't want this repository to be only theoretical.

The concepts will be applied through practical projects such as:

### Batch Data Pipeline

```text
API / Database
      ↓
   Python
      ↓
   Storage
      ↓
    dbt
      ↓
Data Warehouse
      ↓
 Analytics
```

### Orchestrated Pipeline

```text
Source
  ↓
Airflow
  ↓
Ingestion
  ↓
Transformation
  ↓
Data Quality
  ↓
Warehouse
```

### Streaming Pipeline

```text
Application
     ↓
   Kafka
     ↓
Stream Processing
     ↓
Data Storage
     ↓
 Analytics
```

### Cloud Data Platform

```text
Data Sources
     ↓
Cloud Storage
     ↓
Processing
     ↓
Data Warehouse
     ↓
Analytics
```

Projects based on these concepts will be maintained in separate repositories.

---

# 🔍 What I Focus On

When learning a technology, I try to understand more than just how to use it.

I focus on:

* **Reliability** — What happens when something fails?
* **Scalability** — What happens when the data grows?
* **Performance** — How can the system process data efficiently?
* **Data Quality** — Can we trust the output?
* **Observability** — Can we see and understand failures?
* **Security** — Who can access the data?
* **Cost** — How much does the system cost to operate?
* **Maintainability** — Can other engineers understand and change it?

---

#  Progress

This repository is continuously evolving.

### Fundamentals

* [ ] Data Engineering Fundamentals
* [ ] SQL
* [ ] Python
* [ ] Databases

### Data Platform

* [ ] Data Storage
* [ ] Data Modeling
* [ ] Data Transformation
* [ ] Data Quality

### Technologies

* [ ] Airflow
* [ ] dbt
* [ ] Spark
* [ ] Kafka
* [ ] Docker
* [ ] Terraform

### Cloud

* [ ] AWS
* [ ] Azure
* [ ] GCP

### Architecture

* [ ] Data Architecture
* [ ] Distributed Systems
* [ ] Batch Systems
* [ ] Streaming Systems
* [ ] Data Platform Design

---

#  Resources

Most notes are based on:

* Official documentation
* Technical books
* Engineering blogs
* Hands-on experiments
* Open-source projects
* Practical projects

Whenever possible, official documentation is used as the primary reference.

---

#  Learning Process

```text
Learn
  ↓
Understand
  ↓
Practice
  ↓
Build
  ↓
Debug
  ↓
Improve
  ↓
Document
```

This repository will grow alongside my practical experience.

---

#  Goal

The goal is to develop a strong understanding of **modern data engineering** and learn how to design and build reliable data systems.


