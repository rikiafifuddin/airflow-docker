# airflow-docker

Airflow Docker with pip installation using requirement.txt and using DAG from cloned repository

## Requirement

- Install Docker Community Edition (CE).
- Install Docker Compose v1.29.1 or newer.

Note: Older versions of docker-compose do not support all the features required by the Airflow docker-compose.yaml file, so please ensure that your version meets the minimum requirements.

## Installation

1. Clone the Airflow Docker repository.
2. Open the terminal inside the working directory of Airflow Docker.
3. Clone the pws-dag-operation repository, please change volume section in docker compose file same as folder your dag file in my case `pws-dag-operation`.
4. Run the following command: `docker build . --tag extending_airflow:latest`.
5. Run `docker-compose up`.

## Additional pip install requirement
1. Open requirement.txt
2. add library
3. run Installation step 4 and 5

## Open Airflow UI

1. Open `localhost:8080` in your web browser.
2. Login using the following credentials:
   - Username: airflow
   - Password: airflow
   - 
## Disable example DAG

inside docker-compose.yaml change
AIRFLOW__CORE__LOAD_EXAMPLES: 'false'

## Troubleshooting

If you encounter any errors during installation, please contact me or raise issue for assistance.
