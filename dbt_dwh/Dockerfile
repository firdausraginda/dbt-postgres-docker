FROM python:3.10-slim-buster

WORKDIR /app

COPY . /app

ENV DBT_PROFILES_DIR=/app

RUN pip install --upgrade pip
RUN pip install dbt-postgres
RUN dbt deps
