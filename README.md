# Mautic

Mautic Docker Compose configuration

## Installation with Docker

#### 1. Ensure that you have Docker installed

Check that you have the latest [Docker Engine & Docker Compose Plugin](https://docs.docker.com/engine/install/),
installed and running on the machine where you plan to do the installation.

#### 2. Clone the repository

`git clone https://github.com/wmo-raf/nmhs-mautic.git`

#### 3. Create `.env` file from `.env.sample`

```
cd nmhs-mautic
cp .env.sample .env
```

#### 4. Edit the `.env` file and set the environment variables.

See the [Environment Variables](#environmental-variables) section for more details.

#### 5. Build the Docker images

`docker compose build`

#### 6. Run the Docker containers

`docker compose up -d`

You can monitor the logs of the containers with the following command:

`docker compose logs -f`

#### 7. Access Mautic

Open your browser and go to `http://your-ip-address:port` to finish the setup.

## Environmental Variables

Environmental variables for docker compose. All Should be placed in a single `.env` file, saved in the same folder
as `docker-compose.yml` file

| Variable           | Description       |
|--------------------|-------------------|
| MAUTIC_DB_NAME     | Database name     |
| MAUTIC_DB_USER     | Database user     |
| MAUTIC_DB_PASSWORD | Database password |
| MAUTIC_PORT        | Host port to use  |






