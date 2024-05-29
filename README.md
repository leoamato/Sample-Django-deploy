# Django Docker PostgreSQL NGINX Demo

This is a demo project that shows how to deploy a Django application using Docker and connect it to a PostgreSQL database running in another container. Additionally, an NGINX web server is set up in a separate container to serve the Django application.

## Requirements

- Docker
- Docker Compose

## Usage Instructions

1. Clone the Repository

```sh
git clone https://github.com/leoamato/Sample-Django-deploy.git
cd Sample-Django-deploy
```

2. Build and Run the Containers

```sh
docker-compose up --build
```

3. Access the Application

* The Django application will be available at http://localhost:8001.
* The Nginx server will be available at http://localhost:8000.

## NGINX Configuration

The NGINX service is configured to serve the Django application and handle static files. The configuration is defined in the nginx/nginx.conf file.

## Volumes

* postgres_data: Stores PostgreSQL data.
* static_volume: Stores Django static files.

Thank you for using this demo project! If you have any questions or suggestions, feel free to open an issue or submit a pull request.
