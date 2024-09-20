# ELT Pipeline with PostgreSQL, Airflow, and DBT

This repository contains a simple ELT (Extract, Load, Transform) pipeline to transfer data from a source PostgreSQL database to a destination PostgreSQL database, orchestrated using Airflow and with transformations performed by DBT.



## Overview

This ELT pipeline performs the following tasks:
1. **Extract**: Reads data from a source PostgreSQL database.
2. **Load**: Dumps the extracted data into a destination PostgreSQL database.
3. **Transform**: Performs data transformations using DBT.

Airflow is used to orchestrate the workflow, ensuring that the extract, load, and transform tasks are executed in sequence.

## Prerequisites

Before running this pipeline, ensure you have the following installed on your machine:
- [Python 3.8+](https://www.python.org/downloads/)
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Airflow](https://airflow.apache.org/docs/apache-airflow/stable/installation/index.html)
- [DBT](https://docs.getdbt.com/docs/get-started/installation)

## Project Structure
│── README.md # Project documentation │── Dockerfile # Dockerfile to containerize Airflow and DBT │── docker-compose.yml # Docker Compose file for running services │── dags/ │ └── elt_pipeline.py # Airflow DAG to orchestrate the ELT pipeline │── dbt_project/ │ └── dbt_project.yml # DBT project configuration │ └── models/ # DBT models (SQL transformation scripts) │── requirements.txt # Python dependencies for Airflow │── scripts/ │ └── extract.py # Script to extract data from source PostgreSQL │ └── load.py # Script to load data into destination PostgreSQL └── tests/ └── test_pipeline.py # Unit tests for the pipeline





## Getting Started

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/yourusername/elt-pipeline-python-docker.git](https://github.com/Anass-NB/custom-elt-docke)
   cd custom-elt-docker
   docker-compose up














