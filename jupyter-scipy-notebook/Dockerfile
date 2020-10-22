# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
ARG BASE_CONTAINER=jupyter/scipy-notebook
FROM $BASE_CONTAINER

LABEL maintainer="agagosilva"
USER root

RUN pip install --upgrade pip

#Extended file & tensorflow Support
RUN pip install plotly plotly-geo==1.0.0 simpledbf tensorflow
# Switch back to jovyan to avoid accidental container runs as root
USER $NB_UID
