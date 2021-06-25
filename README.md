# dhis2-docker

This document describes the requirement allowing to easily run [dhis2](https://www.dhis2.org/) using [docker](https://www.docker.com/) containers.

## Prerequisites

- [Install Docker Desktop](https://docs.docker.com/desktop/)

## How to have dhis2 running in one command?

Start a terminal and execute docker compose with the default config, Sierra Leone dataset, or use `docker-compose-empty-db.yml` if you want to start with a clean state.

```
docker compose up -d
```

or

```
docker compose -f docker-compose-empty-db.yml up -d
```

Once the container is up, open url http://127.0.0.1:8085 or http://localhost:8085 and connect using username `admin` and password `district` as explained in the [dhis2 documentation](https://www.dhis2.org/doc/snapshot/en/user/html/ch02.html#d5e283)

## Application logs

To access application logs run `docker compose logs -f`.

## Docker images

Docker images can be found at [Docker Hub](https://hub.docker.com/r/dhis2/dhis2-web/ "Docker Hub")

## Using Docker Hub for DHIS2 containers cloud deployment

Docker Hub handles the orchestration of your infrastructure and application containers. The simplest DevOps you'll find without compromising on flexibility, they say...

[Docker Hub is free!](https://hub.docker.com/).

Docker Hub supports several providers:

- [Amazon Web Services](http://aws.amazon.com/ec2/pricing/)
- [Digital Ocean](https://www.digitalocean.com/)
- [Microsoft Azure](https://portal.azure.com/)
- [Google Cloud](https://cloud.google.com/free/)

## Bugs, new requests or contribution

Please submit bugs and feature requests at https://github.com/GwamakaCharles/dhis2/issues

Any other questions contact Gwamaka Charles on Twitter at @GCharles, email at gwamaka.mwamwaja@outlook.com
