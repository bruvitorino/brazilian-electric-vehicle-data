# Brazilian Electric Vehicle Data

An end-to-end Data Engineering project that collects, processes, transforms, and analyzes public Brazilian vehicle fleet data to study the evolution of electric vehicles in Brazil.

The project is designed to simulate a real-world Data Engineering environment, using a Medallion Architecture and technologies such as Python, Apache Spark, Databricks, Delta Lake, SQL, and Power BI.

## Overview

Brazil's electric vehicle fleet has been growing rapidly, creating opportunities to analyze how vehicle electrification is evolving across states, municipalities, and different vehicle categories.

This project builds a complete data pipeline using public data provided by SENATRAN (Secretaria Nacional de Trânsito).

The pipeline will automatically collect source data, preserve the original files, process and transform the datasets using Apache Spark and Delta Lake, and create analytical datasets for dashboards and further analysis.

## Project Goals

The main goal of this project is to build a complete Data Engineering pipeline for Brazilian vehicle fleet data, with a focus on electric vehicle adoption.

The platform will:

- Automatically discover and download public vehicle fleet datasets from SENATRAN.
- Preserve original source files in a Raw layer.
- Ingest and store data using Delta Lake.
- Process large datasets using Apache Spark.
- Clean, standardize, and validate vehicle data.
- Build analytical datasets focused on electric vehicle adoption.
- Provide indicators by year, state, municipality, vehicle type, and fuel type.
- Make curated data available for visualization in Power BI.

## Architecture

The project follows a Medallion Architecture with an additional Raw layer to preserve the original source files.

```text
SENATRAN
    │
    ▼
Data Extraction
    │
    ▼
RAW
Original source files
    │
    ▼
BRONZE
Ingested data stored in Delta Lake
    │
    ▼
SILVER
Cleaned, standardized, and validated data
    │
    ▼
GOLD
Business-ready analytical datasets
    │
    ▼
Power BI
Dashboards and indicators

```
## Tech Stack

### Data Engineering
- Python
- SQL
- Apache Spark
- Delta Lake
- Databricks

### Data Extraction
- Requests
- BeautifulSoup
- Pandas

### Data Visualization
- Power BI

### Development & Version Control
- Git
- GitHub
- Pytest

- ## Project Structure

```text
brazilian-electric-vehicle-data/
│
├── src/
│   ├── extraction/
│   ├── raw/
│   ├── bronze/
│   ├── silver/
│   ├── gold/
│   ├── pipelines/
│   ├── config/
│   └── utils/
│
├── data/
│   ├── raw/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── dashboard/
├── docs/
├── tests/
│
├── README.md
├── requirements.txt
└── .gitignore

```
## Data Source

The project uses public Brazilian vehicle fleet data provided by SENATRAN (Secretaria Nacional de Trânsito).

During the data discovery stage, the available datasets, file formats, update frequency, historical coverage, and download mechanisms will be analyzed before the extraction pipeline is implemented.

## Roadmap

- [x] Sprint 0 — Project foundation and repository setup
- [ ] Sprint 1 — SENATRAN data source discovery
- [ ] Sprint 2 — Automated data extraction
- [ ] Sprint 3 — Raw data layer
- [ ] Sprint 4 — Databricks, Spark and Bronze layer
- [ ] Sprint 5 — Silver data transformation
- [ ] Sprint 6 — Electric vehicle classification
- [ ] Sprint 7 — Gold analytical layer
- [ ] Sprint 8 — End-to-end pipeline and observability
- [ ] Sprint 9 — Data quality and automated tests
- [ ] Sprint 10 — Power BI dashboard
- [ ] Sprint 11 — Documentation and portfolio finalization


