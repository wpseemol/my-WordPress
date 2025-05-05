# WordPress Development Environment

## Setting Up the WordPress Environment

This project uses Docker to set up a WordPress development environment. Follow the steps below to get started:

### Prerequisites

-    Install [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/).

### Installation Steps

1. Clone this repository to your local machine.
2. Navigate to the project directory:
     ```bash
     cd c:\projects\wp-theme-dev
     ```

# WordPress Development Environment

## Setting Up the WordPress Environment

This project uses Docker to set up a WordPress development environment. Follow the steps below to get started:

### Prerequisites

-    Install [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/).

### Installation Steps

1. Clone this repository to your local machine.
2. Navigate to the project directory:
     ```bash
     cd c:\projects\wp-theme-dev
     ```
3. Start the Docker containers:
     ```bash
     docker-compose up -d
     ```
     or
     ```
     docker compose -f file.yml up -d
     ```
4. Access the WordPress site in your browser at [http://localhost:8080](http://localhost:8080).
5. Access phpMyAdmin at [http://localhost:8183](http://localhost:8183) with the following credentials:
     - **Username:** `root`
     - **Password:** `root`

### Stopping the Environment

To stop and remove the containers, run:

```bash
docker-compose down
```

### Additional Notes

-    Ensure the `./wp` and `./mysql` directories exist in your project folder before starting the containers.
-    Modify the `docker-compose.yml` file if you need to customize the environment.
-    Use `docker-compose down --volumes` if you want to remove the associated volumes as well.
