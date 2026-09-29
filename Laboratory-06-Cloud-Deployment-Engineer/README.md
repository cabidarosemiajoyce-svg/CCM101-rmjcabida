# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

Mission 6 focuses on deploying a multi-tier private cloud storage application using Docker Compose. The application consists of a Nextcloud web/application container and a MariaDB database container.

Instead of deploying each container manually, Docker Compose is used to define and manage the application services through a YAML configuration file.

## Objectives

The objectives of this laboratory activity are to:

* Explain the concept of a multi-tier application architecture.
* Understand the purpose and structure of a `docker-compose.yml` file.
* Use a Linux command-line text editor to create configuration files.
* Deploy a multi-container application using Docker Compose.
* Understand Infrastructure as Code (IaC) principles.
* Document the deployment process using Markdown.
* Expand the GitHub Cloud Computing portfolio.

## Commands Executed

The following commands were used during the deployment:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose config
docker-compose up -d
docker-compose ps
docker ps
docker-compose down
```

> **Note:** If the newer Docker Compose syntax is available, `docker compose` may be used instead of `docker-compose`.

## Skills Learned

Through this laboratory activity, I practiced the following skills:

* Docker Compose configuration
* YAML file creation
* Multi-container deployment
* Container networking
* Environment variable configuration
* Linux command-line operations
* Markdown documentation
* Infrastructure as Code
* GitHub portfolio management

## Deployment Architecture

The Mission 6 application uses a two-tier architecture:

```text
+----------------------+
|      Nextcloud       |
|  Web/Application     |
|        Tier          |
+----------+-----------+
           |
           | Docker Network
           |
+----------v-----------+
|       MariaDB        |
|    Database Tier     |
+----------------------+
```

## Evidence

The deployment screenshots are stored in the `screenshots/` directory.

The evidence includes:

1. Docker Compose deployment
2. Nextcloud web interface
3. Docker Compose teardown
