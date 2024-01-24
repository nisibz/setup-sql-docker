# SQL with Docker Setup

This repository provides a straightforward setup for running SQL and phpMyAdmin with Docker using Docker Compose.

## Prerequisites

Ensure that you have the following tools installed on your system:

- Docker
- Docker Compose

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/nisibz/setup-sql-with-docker.git
   cd setup-sql-with-docker
   ```

2. Start the SQL and phpMyAdmin Docker containers:

   ```bash
   docker compose up -d
   ```

3. Access phpMyAdmin:

   Open your web browser and navigate to http://localhost:8080

## Clean up

To stop and remove the containers and volumes created by Docker Compose, execute the following command:

```bash
docker compose down -v
```

Feel free to customize the setup according to your requirements. For any issues or improvements, please open an issue or submit a pull request.
