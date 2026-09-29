# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture is a system that separates an application into two main tiers: the Web/Application Tier and the Database Tier. The Web/Application Tier handles the application and user requests, while the Database Tier stores and manages the data needed by the application.

## The Web/Application Tier

The Web/Application Tier is responsible for providing the user interface and handling HTTP requests from users. In this project, Nextcloud serves as the Web/Application Tier where users can access and interact with the cloud storage application.

## The Database Tier

The Database Tier is responsible for storing and managing persistent data used by the application. In this project, MariaDB serves as the Database Tier and stores information required by the Nextcloud application, including user and application data.

## Why Separate Them?

Separating the web server and database into two containers gives each component a specific responsibility and makes the system easier to manage. It also allows the application and database to be maintained or updated separately instead of placing both components inside one container.
