# FROM quay.io/jupyter/minimal-notebook:latest
FROM quay.io/jupyter/datascience-notebook:2024-11-19
# FROM intel/intel-extension-for-pytorch:2.4.0-pip-jupyter

COPY ./requirements.txt /tmp/requirements.txt
# RUN pip install -r /tmp/requirements.txt

RUN python -m pip install --no-cache-dir \
    --ignore-installed -r /tmp/requirements.txt
