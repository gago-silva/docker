# Start from a core stack version
FROM atavares/miniconda3-rocker-geospatial

LABEL maintainer="agagosilva"


ENV PATH /opt/conda/bin:$PATH

RUN apt-get update -y
RUN apt-get install -y xvfb


RUN pip install pandas

#RUN sudo apt-get build-dep python-imaging
#RUN sudo apt-get install libjpeg62 libjpeg62-dev
RUN pip install Pillow

RUN conda config --add channels conda-forge

RUN conda install \
	matplotlib \
        seaborn \
        plotly \
        plotly-orca \
	tensorflow &&\
	conda clean -tipsy




