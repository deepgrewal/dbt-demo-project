# dbt-demo-project
This repo is a guide to setup DBT using PostgreSQL in windows.

## Table of content
- [Install PostgreSQL](#install-postgresql)
- [Install Python](#install-python)
- [Setup Python](#setup-python)
- [Setup DBT](#setup-dbt)

## Install PostgreSQL
Download and install PostgreSQL
https://www.enterprisedb.com/downloads/postgres-postgresql-downloads

## Install Python
Download and install python
https://www.python.org/downloads/

## Setup Python
### Create a python virtual environment
python -m venv PyEnv

### Activate the virtual environment and upgrade
.\PyEnv\Scripts\activate
pip install --upgrade pip
pip install --upgrade setuptools

## Setup DBT
pip install dbt-postgres

### Initialize new dbt project. 
dbt init

The above command will ask for a project name (In my case it is demo) and a database (In my case it is postgresql).
Once done, it will create a new project in your current repository

### Configure connection to your data warehouse.
cd ~/.dbt

Modify profiles.yaml file

Go inside demo (cd demo) and execute 'dbt run'

