# Start from a core stack version
FROM atavares/miniconda3-rocker-geospatial

LABEL maintainer="agagosilva"


ENV PATH /opt/conda/bin:$PATH

RUN pip install pandas

RUN sudo apt-get build-dep python-imaging
RUN sudo apt-get install libjpeg62 libjpeg62-dev
RUN pip install Pillow

RUN conda config --add channels conda-forge

RUN conda install \
	matplotlib \
        plotly \
        seaborn \
	tensorflow &&\
	conda clean -tipsy




