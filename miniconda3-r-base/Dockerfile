FROM continuumio/miniconda3

RUN apt-get update \
    && apt-get --yes install wget jq git \
    && rm -rf /var/lib/apt/lists/*

# Default environment
RUN conda install --quiet --yes -c conda-forge \
      "r-yaml" \
    && conda clean --all -f -y

RUN conda install --quiet --yes -c conda-forge vim 
RUN conda install --quiet --yes -c conda-forge google-cloud-sdk

