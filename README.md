# Data Pipeline with Python and Object-Oriented Programming

A small data-engineering project that combines data from heterogeneous sources and organizes the workflow into raw, processing, and refined layers.

## Goal

The project demonstrates how a Python pipeline can ingest datasets from different formats, transform them, and produce a consolidated analytical dataset.

## Architecture

```text
JSON source --------\
                     > Raw data -> Python processing -> Refined dataset
CSV source ---------/
```

## Repository structure

```text
pipeline_dados/
├── notebooks/
│   └── exploracao.ipynb
├── raw/
│   ├── dados_empresaA.json
│   └── dados_empresaB.csv
├── refined/
│   └── dados_combinados.csv
└── scripts/
    ├── dados_processados.py
    └── fusao_mercado_fv.py
```

## What this project demonstrates

- ingestion of CSV and JSON data;
- separation between raw and refined datasets;
- data transformation with Python;
- dataset consolidation;
- exploratory analysis with Jupyter;
- organization of pipeline code outside the notebook;
- application of object-oriented programming concepts to data workflows.

## Technologies

- Python
- Pandas
- Jupyter Notebook
- CSV
- JSON

## Suggested execution flow

1. inspect the source files in `pipeline_dados/raw`;
2. run the processing scripts in `pipeline_dados/scripts`;
3. inspect the consolidated output in `pipeline_dados/refined`;
4. use `pipeline_dados/notebooks/exploracao.ipynb` for exploratory analysis.

## Data-engineering concepts

The repository follows a simple layered pattern:

- **Raw** — source data as received;
- **Processing** — Python transformations and consolidation rules;
- **Refined** — cleaned dataset ready for analysis.

This separation makes the workflow easier to understand, debug, and extend.

## Next improvements

- dependency file and reproducible environment;
- command-line entry point;
- automated tests;
- schema validation;
- logging;
- orchestration;
- cloud storage integration;
- CI pipeline.
