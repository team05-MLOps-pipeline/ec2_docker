FROM python:3.10.13
WORKDIR /usr/src/app
COPY . .

RUN apt-get update && apt-get upgrade -y && apt-get install git -y 

RUN python -m pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

WORKDIR ./myapp
RUN git clone https://github.com/team05-MLOps-pipeline/web_stock_chart_flask.git ./

EXPOSE 5000

CMD python main.py


