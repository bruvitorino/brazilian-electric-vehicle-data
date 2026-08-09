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
