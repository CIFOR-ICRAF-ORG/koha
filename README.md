# koha
Library management system
=======
# KOHA Docker

KOHA is the first free and open source Integrated Library System (ILS), designed to streamline library automation. This repository provides a Dockerized environment for running KOHA easily.

## Prerequisites

- A system with [Docker](https://www.docker.com/get-started) installed.
- Familiarity with basic Docker commands.

## Installation

### 1. Build the Docker Image

Build the image using the following command, replacing `your_username/image` with your preferred image name:

```bash
docker build -t your_username/image .
```

After the build process completes, you can verify the image was created successfully by listing all Docker images:

```bash
docker image ls
```
You should see the image listed as your_username/image.

### 2. Spin Up the Container

A sample Docker Compose file is included in the docker folder to help you launch the KOHA container. To start the container using Docker Compose, navigate to the docker folder and run:

```bash
docker-compose up -d
```

This command will start the container in detached mode. You can then view the running container with:

```bash
docker ps
```

### Additional Information

Logs: To view the logs of your KOHA container, use:

```bash
docker-compose logs -f
```
Stopping the Container: To stop and remove the container, run:

```bash
docker-compose down
```

## Contributing

Contributions, bug reports, and feature requests are welcome! Please open an issue or submit a pull request with your suggestions.
