## Apache-Airflow-with-Docker
Apache Airflow is a platform created by the community to programmatically author, schedule and monitor workflows `https://airflow.apache.org/`
### Dependencies Installation
- Pull Apache Airflow Image `docker pull apache/airflow`
- Pull Redis image `docker pull redis`
- Run locally the docker-compose file from `Puckel GitHub`in detached mode `docker-compose -f docker-compose-LocalExecutor.yml up -d `
- Stop the local docker-compose file with `docker-compose -f docker-compose-LocalExecutor.yml down`
`NOTE:` Generate a fernt_key for your project `docker run puckel/docker-airflow python -c "from cryptography.fernet import Fernet; FERNET_KEY = Fernet.generate_key().decode(); print(FERNET_KEY)"`
- Accessing the airflow container `docker exec -it CONTAINER_NAME bash`
### Celery Executor
This is an asyncchronous task queue system that uses a queuing framework such as RabbitMQ or Redis to manage communication between multiple tasks
- Distributes tasks load among multiple worker nodes AND Come with the best ways to scale out the number of workers