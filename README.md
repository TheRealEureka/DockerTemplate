# Docker Template
DockerTemplate is a template for creating a Docker image for a web application. Make sure that port `3306` and `8080` are available. 

## Usage
1. Clone this repository.
2. Place your web application in the `public/` directory.
3. Finaly run `docker-compose up --build` to start the container.
The web server is up at [http://localhost:8080](http://localhost:8080)

## Database
This template uses MariaDB as a database.
To fill the database with data, use the `init/schema.sql` and `init/data.sql` files.

## Composer
You can use composer to install dependencies.

1. Run `docker-compose exec --workdir /app php /bin/bash` to enter the container.
2. Then run `composer install` to install the dependencies.

