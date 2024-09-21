# Docker Environment for WordPress Development + Redis with Docker-Compose

A simplified yet refined Docker Compose workflow that sets up a LEMP network of containers for local WordPress development.

## Usage

To get started, make sure you have [Docker installed](https://docs.docker.com/engine/install/) on your system, and then clone this repository.

Next, navigate in your terminal to the directory you cloned this, and spin up the containers for the web server by running `docker-compose up -d --build`.

After that completes, follow the steps from the [wordpress/README.md](wordpress/README.md) file to get your WordPress installation added in (or create a new blank one).

The following are built for our web server, with their exposed ports detailed:

- **Nginx** - `:80`
- **MariaDB** - `:3306`
- **PHP** - `:9000`

An additional container is included that lets you use the wp-cli app without having to install it on your local machine. Use the following command examples from your project root, modifying them to fit your particular use case.

- `docker-compose run --rm wp user list`

## Thats all! :)
