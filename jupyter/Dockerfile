FROM jupyter/scipy-notebook

USER root

COPY requirements.txt /requirements.txt
RUN pip install --upgrade pip
RUN pip install -r /requirements.txt

ENV PYTHONPATH="${PYTHONPATH}:/app"