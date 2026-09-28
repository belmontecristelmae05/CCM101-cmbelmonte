# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that Docker Compose will create and run. In this laboratory, there are two services: `database` and `app`.

The `database` service uses the MariaDB image, while the `app` service uses the Nextcloud image. Defining both services in the same Docker Compose file allows them to be deployed together.

## How Did the Nextcloud App Container Find the Database Container?

The Nextcloud app container uses the following environment variable:

`MYSQL_HOST=database`

The value `database` refers to the service name defined in the Docker Compose file:

`database:`

Docker Compose allows the containers to communicate using their service names. Therefore, the Nextcloud app container uses `database` to find and communicate with the MariaDB database container.

## What Is the Difference Between `docker run` and `docker-compose up -d`?

The `docker run` command is used to manually create and start an individual Docker container. This was used in Mission 4 when deploying a single container.

The `docker-compose up -d` command uses the `docker-compose.yml` file to create and start multiple services defined in the configuration. In this laboratory, it starts both the Nextcloud application and MariaDB database.

The `-d` option runs the containers in the background.

## Summary

Docker Compose makes it easier to manage multiple related containers using one configuration file. In this laboratory, the `services:` block defined the Nextcloud and MariaDB containers, while `MYSQL_HOST=database` allowed Nextcloud to locate the database container.
