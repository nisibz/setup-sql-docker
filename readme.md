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

3. Update MySQL Username and Password:

- By default, the MySQL username is root, and the password is also root. If you wish to change these credentials, follow these steps:
  - Update the following environment variables under the db service:
  ```
   environment:
      MYSQL_ROOT_PASSWORD: your_new_root_password
      MYSQL_DATABASE: your_new_database_name
  ```

4. Access phpMyAdmin:

   Open your web browser and navigate to http://localhost:8080

## Clean up

To stop and remove the containers and volumes created by Docker Compose, execute the following command:

```bash
docker compose down -v
```

Feel free to customize the setup according to your requirements. For any issues or improvements, please open an issue or submit a pull request.
