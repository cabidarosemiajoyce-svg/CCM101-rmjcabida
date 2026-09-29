# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is an application architecture that separates the system into two main tiers: the web/application tier and the database tier. The web/application tier handles user requests and application processing, while the database tier stores and manages persistent information.

## The Web/Application Tier

The web/application tier is responsible for providing the application that users interact with. It handles requests from users and provides the application's interface.

In Mission 6, **Nextcloud** serves as the web/application tier.

The Nextcloud container is responsible for:

* Providing the web interface
* Receiving HTTP requests
* Processing application requests
* Communicating with the database
* Providing the private cloud storage application

## The Database Tier

The database tier is responsible for storing and managing persistent information used by the application.

In Mission 6, **MariaDB** serves as the database tier.

The MariaDB container is responsible for:

* Storing application data
* Managing database records
* Storing information required by Nextcloud
* Providing database services to the Nextcloud application

## Why Separate Them?

Separating the web/application tier and database tier into different containers makes the system easier to organize and manage. Each container has a specific responsibility, allowing the application and database to be managed independently.

This separation also makes the architecture easier to maintain because changes to one component can be handled without placing both components inside a single container.

## Mission 6 Architecture

The architecture used in this laboratory consists of two main services:

| Tier                 | Service    | Container Image | Purpose                                |
| -------------------- | ---------- | --------------- | -------------------------------------- |
| Web/Application Tier | `app`      | `nextcloud`     | Provides the Nextcloud web application |
| Database Tier        | `database` | `mariadb:10.6`  | Stores application data                |

## Communication Between Containers

The Nextcloud application communicates with MariaDB through the Docker Compose network.

The Compose file contains:

```yaml
MYSQL_HOST=database
```

The value `database` refers to the MariaDB service name defined in the Compose file.

Therefore, the architecture can be represented as:

```text
User
  |
  | HTTP
  v
+----------------------+
|      Nextcloud       |
|    Application Tier  |
|      app service     |
+----------+-----------+
           |
           | MYSQL_HOST=database
           v
+----------------------+
|       MariaDB        |
|     Database Tier    |
|   database service   |
+----------------------+
```

## Summary

The two-tier architecture separates the application from the database. In this laboratory, Nextcloud provides the application interface while MariaDB manages the database. Docker Compose allows both services to be defined and deployed together.
