# Data-Engineering-learning

This repo will have all my personal projects and learning on data engineering concepts.





\# Healthcare Equity \& Expenditure Pipeline



\## Project Overview

This repository contains a research-grade analytics engineering pipeline designed to analyze how regional socio-economic factors, demographic backgrounds, and clinical risk profiles interact to drive catastrophic out-of-pocket medical expenditures in the United States. 



The goal of this project is to build a robust, reproducible data infrastructure that transforms raw public health survey data into analytical models capable of exposing structural healthcare cost disparities.



\## Research Objectives

1\. \*\*Infrastructure:\*\* Build a clean, automated Python data pipeline to ingest, clean, and profile messy public health data.

2\. \*\*Feature Engineering:\*\* Design clinical risk classification matrices by combining biometric markers (BMI) with lifestyle variables.

3\. \*\*Statistical Analysis:\*\* Formulate and mathematically test hypotheses regarding regional spending variations across the United States.



\## Repository Architecture

\- `learning\_basics.ipynb`: Core Python laboratory notebook containing ingestion scripts, data audits, and feature transformation logic.

\- `RESEARCH\_LOG.md`: Active engineering journal tracking daily technical concepts, syntax notes, and environment configurations.



\## Technology Stack

\- \*\*Language:\*\* Python 3

\- \*\*Libraries:\*\* Pandas (Data manipulation), NumPy (Mathematical operations)

\- \*\*Version Control:\*\* Git \& GitHub



## Data Source & Provenance
To ensure research reproducibility, the raw data used in this pipeline is sourced from a verified public health tracking repository:
- **Human-Readable Dataset View:** [Machine Learning with R Datasets - Insurance](https://github.com/stedy/Machine-Learning-with-R-datasets/blob/master/insurance.csv)
- **Direct Data Pipeline Endpoint (Raw CSV):** [Raw Ingestion Link](https://raw.githubusercontent.com/stedy/Machine-Learning-with-R-datasets/master/insurance.csv)

The dataset contains 1,338 fully anonymized patient records mapping demographic, geographic, and lifestyle metrics against annual medical billing charges.
