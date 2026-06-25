<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a Banking Transaction Lakehouse

**Project Link:** [View Project](https://nextwork.ai/projects/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d)

**Author:** Lindokuhle Nyoka  
**Email:** lindokuhle.nyoka03@gmail.com

---

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_8j0ue8b3)

## Building a Banking Transaction Lakehouse

### Project overview and architecture

In this project, I'm building a full medallion architecture pipeline. This matters for banking because they need a system to transform raw data into clean, trustworthy information.

### Setting up Databricks Free Edition

In this step, I'm setting up all my software (Databricks) so I can run my pipeline on it. 

## Configuring the Databricks Environment

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_xg5lxmk6)

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_j6jxbzy9)

## Ingesting Raw Data into the Bronze Layer

### Append-only ingestion with metadata

In this step, I'm building a Bronze Layer, so that I can store all the data.

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_s78dxrwe)

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_ussc90kh)

## Cleaning and Validating Data in the Silver Layer

### Data quality checks and MERGE INTO upserts

In this step, I'm cleaning data from the Bronze layer, so that the data is ready for transformation.

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_43zpzbst)

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_hshon5fw)

## Building Business-Ready Aggregations in the Gold Layer

### Star schema dimensional model

In this step, I'm building the gold layer so that business teams can query and analyse data more easily.

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_odenyboo)

![Image](https://nextwork.ai/lighthearted_indigo_heroic_marjoram/uploads/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d_0vtgty8i)

## Enforcing Data Quality Gates and Audit Trails

### Pipeline health assertions across all layers

In this step, I'm adding quality gates and time travel, so that I can query how the data looked like at any point in history. 

### Delta Lake time travel and audit history

DESCRIBE HISTORY showed me versions, timestamps, user details, and MERGE and CREATE TABLE. This is useful because it is useful for recreating historical reports, and auditing fraud investigations

## Implementing SCD Type 2 for Customer History Tracking

### Why the two-step expire-then-insert pattern

## Reflections and Takeaways

### Key tools and concepts

The key tools I used include PyStark, python and Delta Lake, star schema. Key concepts I learnt include:
Building a complete medallion architecture pipeline (Bronze/Silver/Gold) that ingests raw banking transactions, cleans and deduplicates them with PySpark transformations, and produces business-ready aggregations.
Implementing Delta Lake MERGE INTO for incremental upsert processing with data quality gates, quarantine logic for bad records, and time travel for full audit history.
Designing a star schema dimensional model with fact and dimension tables in the Gold layer, ready for downstream analytics and reporting.

### Time and challenges

This project took me approximately 2 hours. The most challenging part was understanding the code as I have little experience with PySpark and python. 

I did this project today to learn how to be a data engineer and build a full medallion architecture pipeline. Another skill I want to learn is to be proficient in Python and PyStark. I also want to build pipelines without using AI for assistance. 

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/5cc4cf43-c845-4fcd-be4f-5bdff5c2a02d)*
