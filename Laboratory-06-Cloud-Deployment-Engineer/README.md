# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

Mission 6 focuses on deploying a multi-tier private cloud storage application using Docker Compose. The application consists of a Nextcloud web/application container and a MariaDB database container.

Instead of deploying each container manually, Docker Compose is used to define and manage the application services through a YAML configuration file.

## Objectives

At the end of this laboratory activity, I should be able to:

* Explain the concept of a multi-tier application architecture.
* Understand the purpose and structure of a `docker-compose.yml` file.
* Use the Linux command-line text editor `nano` to create configuration files.
* Deploy a multi-container application using Docker Compose.
* Understand Infrastructure as Code (IaC) principles.
* Document deployment procedures using Markdown.
* Continue expanding my Cloud Computing GitHub portfolio.

## Commands Executed

The following commands were used during the laboratory activity:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

Through this laboratory activity, I learned and practiced:

* Multi-tier architecture
* Docker Compose
* YAML configuration
* Linux command-line operations
* Using the `nano` text editor
* Multi-container deployment
* Container networking
* Environment variables
* Infrastructure as Code
* Markdown documentation
* GitHub portfolio management
