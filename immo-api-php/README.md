# Immo API

Simple REST API using Slim v4 MySQL 

## Installation

- Create `.env` from `.env.exemple`
- Update environement variable
- Launch docker-compose
- Copy the sql file into the db container `docker cp ./immo-api-php/create_db.sql [container]:/tmp/script.sql`
- Run `mariadb -u [user] -p [database] < /tmp/script.sql` in the db container to init the data*

## Project Structure

```text
immo-api-php/
├── .env.example       # Template for environment variables
├── .env               # Actual env file (gitignored)
├── docker-compose.yml # App, db and adminer containers
├── create_db.sql      # The initial database dump
├── public/
│   └── index.php      # Slim v4 Entry point
├── src/               # Application logic (Controllers, Models)
└── composer.json      # Dependencies
```

