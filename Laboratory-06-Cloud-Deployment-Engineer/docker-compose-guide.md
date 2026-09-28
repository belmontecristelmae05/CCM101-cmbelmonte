# Docker Compose Guide

## Docker Compose Configuration

The Docker Compose file defines the services required for the Nextcloud deployment. The configuration contains two services: `database` and `app`.

## What Does the `services:` Block Do?

The `services:` block defines the containers that Docker Compose will create and run. In this laboratory, two services are defined:

- `database` - uses the MariaDB image.
- `app` - uses the Nextcloud image.

This allows both containers to be deployed together using one Docker Compose configuration.

## How Does Nextcloud Find the Database?

The Nextcloud application uses the following environment variable:

```yaml
MYSQL_HOST=database
