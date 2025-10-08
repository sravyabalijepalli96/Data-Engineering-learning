# 02. Data Warehousing

## What is a Data Warehouse?
A **data warehouse** (DW) is a central repository of consolidated, historical data from multiple sources. It is designed to support business intelligence (BI), reporting, and analytics, and it's optimized for fast querying of large datasets.

Think of it as a highly organized library. Instead of having books scattered everywhere, a library has a clear system (like the Dewey Decimal System) to make it easy to find what you need. A data warehouse does the same thing for data.

## Key Characteristics
* **Subject-Oriented**: Data is organized around key business subjects (e.g., sales, customers, products) rather than day-to-day transactions.
* **Integrated**: Data is collected from various sources and standardized into a consistent format, which is a major part of the **T** (Transform) in ELT.
* **Time-Variant**: Data warehouses store historical data, so you can analyze trends over time.
* **Non-Volatile**: Data is not updated or deleted once it's in the warehouse. New data is simply added.

## Data Warehouse vs. Data Lake
This is a very common interview topic. The key difference is the data's state when it's stored.

* **Data Warehouse**: Stores **structured, processed data**. It's the final, clean, and ready-to-use version.
* **Data Lake**: Stores **raw, unprocessed data**. It's a vast pool of data in its native format, including structured, semi-structured (like JSON), and unstructured data.
<br>
```mermaid
graph TD
    subgraph Data Sources
        A[App Databases]
        B[APIs]
        C[CSV Files]
    end

    subgraph Data Lake
        D[Raw Data]
        E[Unstructured Data]
    end

    subgraph Data Warehouse
        F[Cleaned Tables]
        G[Aggregated Metrics]
    end

    subgraph Analytics & BI
        H[BI Tools (Tableau)]
        I[Ad-Hoc Analysis]
    end

    A --> |Raw Ingestion| D
    B --> |Raw Ingestion| D
    C --> |Raw Ingestion| D

    D -- "ELT: Transformation" --> F
    F --> G
    G --> H
    G --> I
