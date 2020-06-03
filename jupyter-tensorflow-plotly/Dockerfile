# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
ARG BASE_CONTAINER=jupyter/tensorflow-notebook
FROM $BASE_CONTAINER

LABEL maintainer="agagosilva"
USER root

RUN pip install --upgrade pip
#RUN pip install numpy pandas matplotlib plotly xlrd
#Static Image Export Support
#RUN pip install psutil requests
#Extended Geo Support
RUN pip install plotly plotly-geo==1.0.0
# Switch back to jovyan to avoid accidental container runs as root
USER $NB_UID
