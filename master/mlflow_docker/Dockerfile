FROM python:3.10.13

WORKDIR /usr/src/app

COPY . . 

RUN python -m pip install --upgrade pip
RUN pip install -r requirements.txt

WORKDIR ./myapp

CMD mlflow ui --host 0.0.0.0 --port 5000
