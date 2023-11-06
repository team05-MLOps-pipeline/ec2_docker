FROM python:3.10.13
WORKDIR /usr/src/app
COPY . .

RUN apt-get update && apt-get upgrade -y && apt-get install git -y 

RUN python -m pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

WORKDIR ./myapp
RUN git clone https://github.com/team05-MLOps-pipeline/tick_to_min.git ./


CMD python ./test/test_kafka_to_5bun_copy2.py


