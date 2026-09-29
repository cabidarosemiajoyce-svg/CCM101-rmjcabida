# Docker Compose Guide

## Introduction

Docker Compose is used to define and manage multiple containers as one application. In this laboratory, Docker Compose is used to deploy a Nextcloud application and a MariaDB database.

## What Does the `services:` Block Do?

The `services:` block defines the containers or services that are part of the application.

In the Compose file, two services are defined:

```yaml
services:
  database:
  app:
```

The `database` service uses the MariaDB image, while the `app` service uses the Nextcloud image.

The `database` service represents the database tier, while the `app` service represents the web/application tier.

## How Does the Nextcloud App Find the Database?

The Nextcloud application uses the following environment variable:

```yaml
MYSQL_HOST=database
```

The value `database` refers to the name of the MariaDB service in the Docker Compose file.

Docker Compose creates a network that allows the services in the Compose file to communicate with each other. Because the MariaDB service is named `database`, the Nextcloud container can use `database` as the database host.

## What is the Difference Between `docker run` and `docker-compose up -d`?

The `docker run` command is commonly used to create and start an individual Docker container. Configuration options are normally provided directly in the command.

For example:

```bash
docker run IMAGE
```

On the other hand, `docker-compose up -d` reads the configuration from a `docker-compose.yml` file and creates and starts the services defined in that file.

The `-d` option means that the containers run in the background.

Docker Compose is useful when an application requires multiple containers that need to work together.

## Environment Variables

The Compose file uses environment variables to provide configuration information to the containers.

Examples include:

| Environment Variable  | Purpose                                          |
| --------------------- | ------------------------------------------------ |
| `MYSQL_ROOT_PASSWORD` | Provides the MariaDB root password               |
| `MYSQL_PASSWORD`      | Provides the database user password              |
| `MYSQL_DATABASE`      | Specifies the database name                      |
| `MYSQL_USER`          | Specifies the database user                      |
| `MYSQL_HOST`          | Specifies the database service used by Nextcloud |

## Infrastructure as Code

The `docker-compose.yml` file is an example of Infrastructure as Code (IaC) because the application infrastructure is described in a configuration file.

Instead of manually entering every configuration command, the services and their settings are written in YAML. The same configuration can then be used to deploy the application again.

## Summary

Docker Compose simplifies the deployment of multi-container applications by keeping the configuration in one YAML file. In Mission 6, the Nextcloud application and MariaDB database are defined as separate services that communicate through the Docker Compose network.
