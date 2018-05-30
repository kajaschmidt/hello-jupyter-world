FROM jupyter/datascience-notebook

RUN python --version

RUN conda install --quiet --yes -c \
    conda-forge osmnx dask

COPY requirements.txt /jupyter/requirements.txt
WORKDIR /jupyter
RUN pip install -r requirements.txt

VOLUME /notebooks
WORKDIR /notebooks
