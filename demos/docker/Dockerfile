FROM ubuntu

RUN apt-get update
RUN apt-get install python

RUN pip install flask
RUN pip install flask-mysql

COPY . /opt/source-code

ENTRYPOINT FALSK_APP=/opt/source-code/app.py flask run 

# docker build Dockerfile -t username/app