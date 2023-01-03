FROM python:3.9.16-alpine3.16
WORKDIR /code
ENV FLASCK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
RUN apk add --no-cahe gcc musl-dev linux-headers
COPY requirements.txt requierements.txt
RUN pip install -r requierements.txt
EXPOSE 5000
COPY ..
CMD ["flask","run"]
