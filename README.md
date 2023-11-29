# Apache Airflow


export AIRFLOW_HOME=. <br>
or <br>
set AIRFLOW_HOME=.<be>


<br><be>

airflow db init <br>
<br>

create a new file .env and add the following lines
<br><br>

AIRFLOW_IMAGE_NAME=apache/airflow:2.4.2 <br>
AIRFLOW_UID=50000
<br>

give docker-compose.yaml file

docker-compose up -d

create Admin user using below command:

docker-compose run airflow-worker airflow users create --role Admin --username admin --email admin --firstname admin --lastname admin --password admin
