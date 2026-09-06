# Data Engineering Fundamentals

This section covers the fundamental concepts behind modern data engineering.

The goal is to understand **how data moves through a system**, how it is stored and transformed, and what makes a data platform reliable and scalable.

---

## 📚 Topics

### 1. What is Data Engineering?

Understanding:

* What data engineering is
* What a data engineer does
* Data engineering vs data analytics
* Data engineering vs data science
* Common responsibilities
* Modern data platforms

---

### 2. Data Engineering Lifecycle

Understanding the typical journey of data:

```text
Sources
   ↓
Ingestion
   ↓
Storage
   ↓
Transformation
   ↓
Serving
   ↓
Analytics / Applications
```

---

### 3. ETL vs ELT

Understanding two common approaches to moving and transforming data.

**ETL**

```text
Extract
   ↓
Transform
   ↓
Load
```

**ELT**

```text
Extract
   ↓
Load
   ↓
Transform
```

Topics include:

* When to use ETL
* When to use ELT
* Advantages and disadvantages
* Modern ELT architecture

---

### 4. Batch vs Streaming

Understanding different ways of processing data.

**Batch**

```text
Data
 ↓
Collect
 ↓
Process periodically
```

**Streaming**

```text
Event → Event → Event → Event
          ↓
      Process continuously
```

Topics include:

* Batch processing
* Real-time processing
* Micro-batching
* Use cases
* Trade-offs

---

### 5. Data Pipelines

Understanding how data pipelines are designed and operated.

Topics include:

* Pipeline components
* Dependencies
* Scheduling
* Retries
* Failure handling
* Idempotency
* Monitoring
* Data quality
* Pipeline reliability

---

### 6. Data Lakes

Understanding how raw and processed data can be stored at scale.

Topics include:

* Object storage
* Raw data
* Structured and unstructured data
* Data lake layers
* Partitioning
* File formats
* Data lake architecture

---

### 7. Data Warehouses

Understanding systems designed primarily for analytical workloads.

Topics include:

* OLTP vs OLAP
* Analytical workloads
* Tables
* Schemas
* Fact and dimension tables
* Data warehouse architecture

---

### 8. Data Lakehouse

Understanding the combination of data lake flexibility and warehouse capabilities.

Topics include:

* Lakehouse concept
* Why lakehouses exist
* Data lake vs warehouse vs lakehouse
* Table formats
* ACID transactions
* Schema management

---

### 9. Data Formats

Understanding how data is represented and stored.

Common formats:

* CSV
* JSON
* Parquet
* Avro

Topics include:

* Row vs column storage
* Compression
* Schema
* Performance
* When to use each format

---

### 10. Schemas

Understanding how the structure of data is defined.

Topics include:

* Schema
* Data types
* Schema design
* Schema validation
* Schema evolution
* Backward compatibility
* Forward compatibility

---

### 11. Data Quality

Understanding how to make data trustworthy.

Important dimensions include:

* Accuracy
* Completeness
* Consistency
* Uniqueness
* Validity
* Freshness

Also:

* Data validation
* Data testing
* Data contracts
* Monitoring

---

### 12. Data Lineage

Understanding where data comes from and where it goes.

Example:

```text
API
 ↓
Raw Data
 ↓
Staging
 ↓
Transformation
 ↓
Data Warehouse
 ↓
Dashboard
```

Lineage helps answer:

> Where did this data come from?

and:

> What will be affected if this table changes?

---

### 13. Metadata

Metadata is information about data.

Examples:

* Table name
* Column name
* Data type
* Data owner
* Data source
* Data freshness
* Data lineage
* Business definition

Understanding metadata is important for building maintainable data platforms.

---

# 🧠 Learning Approach

For each topic, I will focus on:

```text
What is it?
     ↓
Why do we need it?
     ↓
How does it work?
     ↓
When should we use it?
     ↓
What are the trade-offs?
     ↓
How is it used in production?
```

---

# 🏗️ Big Picture

All of these concepts come together to form a modern data platform:

```text
                 DATA SOURCES
                      │
          ┌───────────┴───────────┐
          │                       │
       Databases                APIs
          │                       │
          └───────────┬───────────┘
                      ↓
                 INGESTION
                      ↓
                DATA STORAGE
                      ↓
              TRANSFORMATION
                      ↓
              DATA WAREHOUSE
                      ↓
                  ANALYTICS
```

Supporting the entire platform:

```text
Data Quality
     +
Security
     +
Monitoring
     +
Lineage
     +
Governance
     +
Cost Management
```

---

## 🎯 Goal

Build a strong understanding of the fundamentals before moving into specific tools such as:

```text
SQL
Python
PostgreSQL
Airflow
dbt
Spark
Kafka
AWS / Azure / GCP
```

> **Understand the data problem first. Choose the technology second.**
