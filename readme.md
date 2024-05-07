# Flask Application with PostgreSQL

This project is a simple Flask application configured to run with Docker and connected to a PostgreSQL database. It demonstrates the basics of setting up a Flask application with Docker and utilizing a relational database.

## Prerequisites

Before you begin, ensure you have met the following requirements:
- Docker installed on your machine (Docker Desktop for Windows/Mac or Docker Engine for Linux).
- Docker Compose installed if it's not already included in your Docker Desktop installation.

## Project Structure directory

```
back_end|
        |-app.py
        |-Dockerfile
        |-requirements.txt
docker-compose.yml
readme.md
```

- `app.py`: The Flask application file with a simple route.
- `Dockerfile`: Instructions for Docker on how to build the Flask app's image.
- `requirements.txt`: Python libraries required for the Flask app.
- `docker-compose.yml`: Configuration for Docker services including the Flask app and PostgreSQL database.

## Setup and Running

1. **Build and Run Docker Containers**
    To build and run the Docker containers, navigate to the root directory of the project and run:
    ```bash
    docker-compose up --build
    ```

2. **Accessing the Application**
    Once the Docker containers are running, access the Flask application at:
    ```
    http://localhost:5000/
    ```

3. **Shutting Down**
    To stop and remove the Docker containers, you can use:
    ```bash
    docker-compose down
    ```

## Features
 
- Flask web server running in a Docker container.
- PostgreSQL database integration.
- CORS enabled via `flask_cors`.

>[!CAUTION]
>First the Docker Compose image must be built and run, and only then can the server be created in pgAdmin, otherwise it would lead to errors <br> 👉 TAKE A LOOK on my repo [DockerFlask_pgAdmin](https://github.com/JungleKiosk/DockerFlask_pgAdmin)


