# syntax=docker/dockerfile:1.4
FROM --platform=linux/amd64 python:3.10-alpine AS builder

WORKDIR /app

COPY requirements.txt /app
RUN pip3 install -r requirements.txt

COPY . /app

ENTRYPOINT ["python3"]
CMD ["app.py"]