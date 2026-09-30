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

The `docker run` command is used to create and start a container individually. The user must specify the necessary settings in the command.

The `docker-compose up -d` command uses the `docker-compose.yml` file to create and start multiple related containers together. In this activity, it starts both the Nextcloud application and the MariaDB database using one command.

The `-d` option runs the containers in the background, allowing the terminal to be used for other commands.
