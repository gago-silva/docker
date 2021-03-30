# Start from a core stack version
FROM atavares/miniconda3-rocker-geospatial

LABEL maintainer="agagosilva"


ENV PATH /opt/conda/bin:$PATH

RUN pip install Pillow lxml Cython opencv-python laspy simpledbf

RUN conda config --add channels conda-forge

RUN conda install \
	pandas \
	matplotlib \
        plotly \
        seaborn \
        gdal \
	cartopy \
	tensorflow &&\
	conda clean -tipsy

RUN pip install xarray rioxarray geopandas earthpy


