FROM python:3.7-slim-stretch

RUN pip install --upgrade pip && pip install protobuf==3.20.1
RUN pip install "urllib3<2.0"

# Install mlflow
RUN python -m pip install --upgrade pip mlflow==1.4.0

# Expose mlflow port
EXPOSE 1234

# Define entry point
ENTRYPOINT mlflow server --host 0.0.0.0 --port 1234