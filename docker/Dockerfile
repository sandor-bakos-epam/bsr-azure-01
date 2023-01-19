FROM mcr.microsoft.com/azureml/openmpi4.1.0-ubuntu20.04

RUN apt-get update

RUN conda install python=3.9

# https://github.com/Azure/MachineLearningNotebooks/issues/1110
RUN python -m pip install --upgrade pip==20.2.4

COPY ./docker/requirements.txt .

RUN python -m pip install --no-cache-dir -r requirements.txt