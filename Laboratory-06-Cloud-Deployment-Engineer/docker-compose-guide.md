# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that are part of the application. In the YAML file, it contains two services: `database` for the MariaDB container and `app` for the Nextcloud container.

## How Did the Nextcloud App Container Find the Database Container?

The Nextcloud app container uses the `MYSQL_HOST` environment variable to identify the database container. In the YAML file, `MYSQL_HOST=database` tells Nextcloud to connect to the MariaDB container using the service name `database`.

## What is the Difference Between `docker run` and `docker-compose up -d`?

The `docker run` command is used to create and start an individual Docker container, with its configuration provided directly in the command. In comparison, `docker-compose up -d` reads the `docker-compose.yml` file and creates and starts multiple containers defined in the `services:` block. The `-d` option runs the containers in the background.
