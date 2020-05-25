
FROM agagosilva/jupyter-plotly

LABEL maintainer="agagosilva"
USER root

# Install all OS dependencies for fully functional notebook server
RUN pip install --upgrade pip
RUN pip install dash

# Switch back to jovyan to avoid accidental container runs as root
USER $NB_UID
