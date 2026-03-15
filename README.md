# CS544 P8: Google Cloud Services

**Course:** CS544 — Big Data Systems, UW-Madison (Fall 2025)

## Overview

Used four **Google Cloud Platform** services to analyze all schools in Wisconsin. Built a Dataform pipeline to bring geographic and school data into **BigQuery**, then answered analytical questions using SQL.

## Learning Objectives

- Store and access files on Google Cloud Storage (GCS)
- Build data pipelines with Dataform (dbt-like transformations)
- Query large datasets with BigQuery SQL
- Join public geographic datasets with custom data in BigQuery

## Architecture

```
Wisconsin Schools CSV
        │
        ▼ upload
Google Cloud Storage (GCS)
        │
        ▼ Dataform pipeline
BigQuery Dataset
  ├── schools table
  ├── geographic data (public)
  └── joined views
        │
        ▼ SQL queries
Analysis Results
```

## Tech Stack

![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat&logo=googlebigquery&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

## Project Structure

```
p8/
├── p8.ipynb            # Main notebook: GCS upload + BigQuery queries
├── dataform/           # Dataform pipeline definitions
│   ├── sources.sqlx    # GCS data source
│   └── schools.sqlx    # Transformed table
└── README.md
```

## Key Analysis

Answered geographic and statistical questions about Wisconsin schools including district distributions, enrollment trends, geographic clustering, and public vs private school comparisons using BigQuery SQL joins with public geographic datasets.

## Author

**Rakshith Sriraman Krishnaraj** · MS CS @ UW-Madison · [LinkedIn](https://www.linkedin.com/in/rakshith-s-k-95b550151/)
