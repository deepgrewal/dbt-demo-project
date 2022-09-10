# dbt-demo-project
This repo is to demo the use of dbt using PostgreSQL

<img src="image.png" />

Download and install PostgreSql. I use Windows Subsystem for Linux. So I installed postgres in Ubuntu
https://www.enterprisedb.com/downloads/postgres-postgresql-downloads

Create a python virtual environment
python -m venv PyEnv

Activate the virtual environment and upgrade
.\PyEnv\Scripts\activate
pip install --upgrade pip
pip install --upgrade setuptools

Install dbt
pip install dbt-postgres

Initialize new dbt project. 
dbt init

The above command will ask for a project name (In my case it is demo) and a database (In my case it is postgresql).
Once done, it will create a new project in your current repository

Configure connection to your data warehouse.
cd ~/.dbt

Modify profiles.yaml file

Go inside demo (cd demo) and execute 'dbt run'

