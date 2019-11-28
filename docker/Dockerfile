FROM jupyter/datascience-notebook
USER root
COPY docker/requirements.txt /tmp/
RUN pip install -r /tmp/requirements.txt
RUN jupyter contrib nbextension install

