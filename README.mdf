
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Deploy Wordpress on Localhost and in Production using Docker Compose

Related blog post:

  - [WordPress Local Development Using Docker
    Compose](https://www.datanovia.com/en/lessons/wordpress-local-development-using-docker-compose/):
    Deploy Wordpress on localhost using docker
  - [Docker WordPress Production
    Deployment](https://www.datanovia.com/en/lessons/docker-wordpress-production-deployment/):
    Step-by-step guide to deploy WordPress online using docker-compose
  - [Using Docker WordPress Cli to Manage WordPress
    Websites](https://www.datanovia.com/en/lessons/using-docker-wordpress-cli-to-manage-wordpress-websites/):
    Commande line interface for managing a WordPress website

The installation tool kit, provided here, include:

  - Nginx web server
  - MariaDB/MySQL used for Wordpress database
  - phpMyAdmin interface to connect to your MySQL database
  - WP-Cli: Wordpress Command Line Interface
  - Makefile directives for automatization.

You can automatically deploy a local docker wordpress site in 5 minutes
using the following commands:

``` bash
# Download a wordpress docker-compose example
git clone https://github.com/dinhduan2710/docker-wordpres.git
cd wordpress-docker-compose
# Build and start installation
docker-compose up -d --build
```

Visit your site at <http://localhost> and your database via phpMyAdmin
at <http://localhost:8080>.

Default identification for your wordpress website admin:

  - `Username: wordpress` and
  - `Password: wordpress`

Default identification for the phpMyAdmin interface:

  - `Username: root` and
  - `Password: password`

**Useful set of commands to know**:

``` bash
# Stop and remove containers
docker-compose down
# Build, and start the wordpress website
docker-compose up -d --build
# Reset everything
docker-compose down
rm -rf certs/* certs-data/* logs/nginx/* mysql/* wordpress/*
```

## References

  - [WordPress: with Nginx web server in
    Docker](https://github.com/mjstealey/wordpress-nginx-docker)
  - [Quickstart: Compose and
    WordPress](https://docs.docker.com/compose/wordpress/)

## Construct

### Essential folders:

- `mysql`: MySQL database files for MariaDB
- `wordpress`: WordPress web files
- wpcli contains a Dockerfile example to build WordPress CLI.

### Essential files:

- `.env file`: contain the environment variables required for the wordpress installation
- `docker-compose.yml`: WordPress docker compose application services
- `Makefile`: Set of simple bash command lines to build, install and configure WordPress, as well as, to start and stop the docker containers.