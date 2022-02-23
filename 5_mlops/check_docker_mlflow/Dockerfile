FROM python:3.8.9-slim-buster

COPY . /app
WORKDIR /app
ENV PYTHONPATH=/app
ENV PYTHONUNBUFFERED=1

RUN pip install mlflow>=1.0 && \
    pip install numpy && \
    pip install scikit-learn && \
    pip install matplotlib

