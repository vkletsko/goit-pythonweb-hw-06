# goit-pythonweb-hw-06

Fullstack Web Development with Python

Master of degree from University

Building:

```shell
cd goit-pythonweb-hw-06
python3 -m pip install psycopg2-binary
poetry install
```

## Setup

1. Start the PostgreSQL

   ```shell
   docker run --name hw06_postgres -p 5432:5432 -e POSTGRES_PASSWORD=mypostgrespasswd -d postgres
   ```

2. Apply Migrations

   ```shell
   alembic upgrade head
   ```

3. Seed the Database with Fake Data

   ```shell
   python3 seed.py
   ```
   
## Usage
### Selects

```shell
python3 my_select.py
```

## Stopping PostgreSQL Docker

```shell
docker stop hw06_postgres
docker rm hw06_postgres
```