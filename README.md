# docker-php-nginx-postgres-pga-redis-compose
Docker Compose configuration to run PHP 7.2 with Nginx, PHP-FPM, Composer, Supervisord, PostgreSQL 10, Redis, and pgAdmin4

# Install prerequisites

You will need:

* [Docker CE](https://docs.docker.com/engine/installation/)
* [Docker Compose](https://docs.docker.com/compose/install)
* Git (optional)

## How to use it

Checkout the repository or download the sources.

Simply run following commands:

`cp .env.example .env` (at the first launch)

`docker-compose up`

And you are done.

Nginx will be available on `localhost:80` and pgAdmin4 on `localhost:8080`

#### pgAdmin default credentials:

email: `richard@example.com`

password: `secret`

#### Windows

Use external docker volume in Windows (see docker-compose.yml)

Create volume:

`docker volume create postgres_persistence`

# Documentation for used docker images:

* [webdevops/php-nginx](https://dockerfile.readthedocs.io/en/latest/content/DockerImages/dockerfiles/php-nginx.html)
* [sameersbn/postgresql](https://hub.docker.com/r/sameersbn/postgresql/)
* [dpage/pgadmin4](https://hub.docker.com/r/dpage/pgadmin4/)
* [redis](https://hub.docker.com/_/redis/)

# Contribution

Pull requests are always welcome :)

# See also

* [Laradock - Docker PHP development environment](https://github.com/laradock/laradock/)
