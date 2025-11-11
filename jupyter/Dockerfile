FROM python:3.9-slim

WORKDIR /app

# Install dependencies
RUN apt-get update && apt-get install -y build-essential curl libpq-dev && rm -rf /var/lib/apt/lists/*

# Install Jupyter and SQL-related packages
RUN pip install --no-cache-dir jupyter jupysql psycopg2-binary pandas sqlalchemy

# Expose Jupyter port
EXPOSE 8888
