USER root

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    build-essential \
    libssl-dev \
    libffi-dev \
    libblas-dev \
    liblapack-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

USER airflow

# Install additional dependencies if needed
# RUN pip install <your-dependencies>

ENTRYPOINT ["entrypoint.sh"]
