# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture separates an application into two main parts: the web/application tier and the database tier. In this laboratory, Nextcloud is used as the application tier while MariaDB is used as the database tier.

## The Web/Application Tier

The web/application tier provides the application that users access through a web browser. In this laboratory, the Nextcloud container handles the web interface and HTTP requests. It is exposed through port `8080`.

## The Database Tier

The database tier stores persistent information required by the application. MariaDB is used in this laboratory to store database information needed by Nextcloud, including user and application data.

## Why Separate Them?

Separating the application and database into different containers makes the system easier to manage and organize. Each container has a specific responsibility, and the services can communicate with each other through the Docker Compose network.
