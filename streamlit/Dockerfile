FROM python:3.10.6
# Base docker image of python 3.x

RUN pip install --upgrade pip
# Upgrade pip package

WORKDIR /
# Change working dir to app

COPY ./streamlit/ /streamlit/

# COPY ../apis.py ../schemas.py ../requirements.txt ../metadata.db ../aws_logging.py /app/

# COPY ../Authentication /app/Authentication

# COPY ../Util/ /app/Util/

ENV JWT_SECRET='damg_7225_big_data'
ENV DbGeo='/fastapi/data/GEOSPATIAL_DATA.db'
ENV DbPath='/fastapi/data'
ENV DbUser='/fastapi/data/USER_DATA.db'
ENV AWS_ACCESS_KEY_ID = "AKIA3EJL4FYTQOGZWUOB"
ENV AWS_SECRET_ACCESS_KEY = "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"
ENV LOG_GROUP_NAME = "damg7245_Assignment1"
ENV LOG_STREAM_NAME_AWS = "aws_services"
ENV LOG_STREAMLIT_NAME = "streamlit_ui"
ENV BUCKET_NAME = "damg7245-s3-storage"

RUN pip install -r ./streamlit/requirements.txt
WORKDIR /streamlit/
EXPOSE 8501
## Expose a port inside the container on which services run
#
CMD ["streamlit", "run", "Home.py"]
# gunicorn command to run the service with 4 worker nodes binding localhost/0.0.0.0 on port 8000 refering app inside the main.py
