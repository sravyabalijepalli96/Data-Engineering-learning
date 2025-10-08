# 01. The Data Pipeline Lifecycle

## What is a Data Pipeline?
A data pipeline is a series of steps for moving data from a source system to a destination where it can be analyzed. Think of it like a plumbing system for data.

## Key Steps
There are typically three main steps:

1.  **Extract**: Pulling raw data from a source (like a database or API).
2.  **Load**: Putting that raw data into a storage system (like a data warehouse).
3.  **Transform**: Cleaning, joining, and structuring the data so it's ready for analysis.

## My First Diagram
This diagram shows the ELT (Extract, Load, Transform) process, which is the modern standard for data pipelines.

```mermaid
graph TD
    A[Source System: Cin7] --> B(Extract: Fivetran)
    B --> C[Load: Snowflake PRD]
    C --> D(Transform: dbt in DEV/QA)
    D --> E[Final Data Model]
