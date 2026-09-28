# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory focused on deploying a multi-tier private cloud storage application using Docker Compose. The application used Nextcloud as the web application and MariaDB as the database. Instead of deploying the containers separately, Docker Compose was used to define and deploy the services together using a YAML configuration file.

## Objectives

- Understand multi-tier application architecture.
- Understand the purpose and structure of a `docker-compose.yml` file.
- Use a Linux command-line text editor to create configuration files.
- Deploy a multi-container application using Docker Compose.
- Access a Nextcloud web application through port 8080.
- Document Infrastructure as Code (IaC) concepts.
- Practice maintaining a Cloud Computing GitHub portfolio.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
