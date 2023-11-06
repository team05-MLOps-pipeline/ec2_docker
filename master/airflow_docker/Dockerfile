FROM apache/airflow:2.7.2-python3.10

COPY requirements.txt /tmp/requirements.txt
USER root

RUN umask 0002
RUN apt-get update && apt-get -y install gcc g++

USER airflow


RUN pip install --no-cache-dir -r /tmp/requirements.txt

