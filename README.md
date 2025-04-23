## Apache-Airflow-with-Docker
Apache Airflow® is a platform created by the community to programmatically author, schedule and monitor workflows `https://airflow.apache.org/`
### Dependencies Installation
- Pull Apache Airflow Image `docker pull apache/airflow`
- Pull Redis image `docker pull redis`
- Run locally the docker-compose file from `Puckel GitHub`in detached mode `docker-compose -f docker-compose-LocalExecutor.yml up -d `
- Stop the local docker-compose file with `docker-compose -f docker-compose-LocalExecutor.yml down -d`
### 