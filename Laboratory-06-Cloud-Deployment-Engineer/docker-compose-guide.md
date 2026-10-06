# Docker Compose Guide

This guide explains the `docker-compose.yml` file used to deploy Nextcloud and MariaDB.

## The Compose File

```yaml
version: '3'

services:
  database:
    image: mariadb:10.6
    environment:
      - MYSQL_ROOT_PASSWORD=cloudnova_root
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user

  app:
    image: nextcloud
    ports:
      - 8080:80
    environment:
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user
      - MYSQL_HOST=database
```

## What does the `services:` block do?

The `services:` block lists every container that makes up the application. Each entry under it is one service with its own image, port mappings, and environment variables. In this file there are two services: `database` (MariaDB) and `app` (Nextcloud). Docker Compose reads this block and creates and starts one container for each service.

## How did the Nextcloud app container find the database container?

The app container found the database through the `MYSQL_HOST=database` environment variable. Docker Compose automatically puts all services in the same file on a shared network, and each service name works as a hostname through Docker's built-in DNS. So when Nextcloud connects to the host `database`, Docker resolves that name to the IP address of the MariaDB container. No IP address needed to be written by hand.

## What is the difference between `docker run` and `docker-compose up -d`?

| `docker run` | `docker-compose up -d` |
|---|---|
| Starts one container per command | Starts all services defined in the file |
| Options are typed manually every time | Options are saved in `docker-compose.yml` |
| Networking between containers must be set up manually | A shared network is created automatically |
| Easy to make typos and hard to repeat | Repeatable and easy to share or version control |

In both cases, `-d` means "detached", so the containers run in the background and the terminal stays free.
