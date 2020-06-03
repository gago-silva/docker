# Start from a core stack version
FROM atavares/miniconda3-rocker-geospatial

LABEL maintainer="agagosilva"


ENV PATH /opt/conda/bin:$PATH

RUN conda config --add channels conda-forge

RUN conda install \
        plotly \
	tensorflow && \
	conda clean -tipsy




