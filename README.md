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



## Getting Started

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Anass-NB/custom-elt-docker
   cd custom-elt-docker
   docker-compose up

