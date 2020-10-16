# App-PostgreSQL

## First Time Prerequisites

1. `rm ./Data/postgresql/.gitkeep`

## Running the Containers

1. Update the following volume mount in [docker-compose.yml](./Docker/docker-compose.yml)
    * `./Data/postgresql:/var/lib/postgresql/data`
2. Update the following environment variables in [docker-compose.yml](./Docker/docker-compose.yml)
    * `- POSTGRES_USER=changeme`
    * `- POSTGRES_PASSWORD=changeme`
    * `- POSTGRES_DB=changeme`
3. Run `docker-compose -f ./Docker/docker-compose.yml up -d`
