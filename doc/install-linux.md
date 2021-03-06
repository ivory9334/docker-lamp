# Docker toolbox on Linux

## Prerequisites
* [Docker](https://docs.docker.com/engine/installation/linux/)
* [Docker-compose](https://docs.docker.com/compose/install/)

## Init
```
$ docker network create --driver bridge lamp-network
$ cp docker-compose.yml.dist docker-compose.yml
```

You would change the database folder to point to another location than default one (/var/lib/boot2docker). 

Then:

```
$ docker-compose -f /path/to/docker/docker-compose up -d
```

That's all !

## What's next?
* [Post configuration](config.md)