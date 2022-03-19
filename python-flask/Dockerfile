FROM python:alpine3.14

WORKDIR /opt

COPY app/ ./

RUN pip3 install -r requirements.txt

ENV FLASK_APP /opt/app.py
ENV FLASK_RUN_HOST 0.0.0.0
ENV FLASK_RUN_PORT 8080
ENV FLASK_ENV development

EXPOSE ${FLASK_RUN_PORT}

ENTRYPOINT flask run
