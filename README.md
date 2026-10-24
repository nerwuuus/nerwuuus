# 👋 Hi, I'm Patryk Żychlewicz

Welcome to my GitHub portfolio! I'm a **Marketing Science Analyst** working with data pipelines, ETL processes, large-scale datasets, and marketing analytics (Marketing Mix Modelling).

My current focus is on developing stronger **Data Engineering** skills through practical work with Python, SQL, PostgreSQL, Docker, Apache Airflow, Polars, and PySpark.

## 💼 Current work

Since January 2026, my work has included:

- Building and maintaining ETL pipelines in **Pentaho** for marketing analytics and reporting workflows
- Processing and validating large CSV and Excel datasets, including nationwide sales datasets with **36+ million records**
- Developing transformation logic for joins, aggregations, mapping tables, pivot/unpivot operations, data standardization, and metric/value-based structures
- Debugging ETL issues and validating data quality across fact tables, dimension tables, mapping tables, and downstream datasets
- Using **PostgreSQL** for data transformation, validation, troubleshooting, and preparation
- Translating existing **R-based data preparation logic** into PostgreSQL queries and Pentaho transformations
- Using **Python and pandas** for ad hoc validation, exploration, and troubleshooting
- Preparing analysis-ready datasets for reporting, BI, and **Marketing Mix Modeling (MMM)**
- Working with regression-based MMM workflows and supporting data preparation for statistical modeling
- Collaborating with international teams on large-scale analytics and data preparation projects

## 🌦️ Weather Data Processing

My main personal Data Engineering project is an end-to-end pipeline built around the **NOAA Global Historical Climatology Network Daily (GHCN-Daily)** dataset.

The project processes more than **400 million weather observations** and has evolved from a small ETL exercise into a broader Data Engineering learning environment.

🔗 [Weather Data Processing project](https://github.com/nerwuuus/data-toolkit/tree/main/weather_data_processing)

### Main areas covered

- PostgreSQL **Staging → Bronze → Silver → Gold** architecture
- Historical bootstrap and recurring incremental loading
- Natural keys, `UNIQUE` constraints, and `ON CONFLICT`
- Automated Data Quality checks
- Airflow orchestration
- Docker
- Pandas, Polars, Polars Lazy, and PySpark
- CSV vs Parquet and Pandas vs Polars benchmarks
- PostgreSQL performance experiments
- Automated retrieval and processing of new NOAA observations

The recurring pipeline is orchestrated by Airflow:

`NOAA → incremental batch → Staging → Bronze → Silver → Gold → Data Quality`

### Project structure

```text
weather_data_processing/
├── 00_raw_data/                  # Raw and intermediate NOAA data
├── 01_scripts/                   # Python, SQL, notebooks and ETL scripts
│   └── tests/                    # Development and test scripts
├── 02_plots/                     # Generated visualizations
├── 03_docker/                    # Docker configuration and documentation
├── 04_data_quality_checks_sql/   # Manual and automated SQL DQ checks
├── 05_postgres_optimization/     # PostgreSQL performance and indexing experiments
├── 06_airflow/                   # Airflow DAGs and configuration
├── docs/                         # Architecture and project documentation
├── compose.yaml                  # Docker Compose infrastructure
├── requirements.txt              # Python dependencies
└── README.md                     # Full project documentation
```

## 🧰 Technologies

- **SQL / PostgreSQL**
- **Python**
- **Pandas**
- **Polars**
- **PySpark**
- **Pentaho**
- **Apache Airflow**
- **Docker / Docker Compose**
- **Apache Parquet**
- **R**
- **Git / GitHub**

## 📚 Current learning focus

I'm currently strengthening my foundations in:

- Advanced SQL and window functions
- Python
- Data Engineering architecture
- PySpark

Later, I plan to expand the weather pipeline with **cloud storage and Databricks**.

## 📫 Let's connect

Feel free to explore my projects or connect with me on [LinkedIn](https://www.linkedin.com/in/patrykzychlewicz/).
