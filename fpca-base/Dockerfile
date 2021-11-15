FROM continuumio/miniconda3

RUN apt-get update \
    && apt-get --yes install wget jq git \
    && rm -rf /var/lib/apt/lists/*

# Default environment
RUN conda install --quiet --yes \
      -c conda-forge \
      "r-cowplot" \
      "r-dplyr" \
      "r-fda" \
      "r-ggplot2" \
      "r-logger" \
      "r-ncdf4" \
      "r-R6" \
      "r-readr" \
      "r-stringr" \
      "r-tidyr" \
    && conda clean --all -f -y

# RUN R CMD install --clean --no-html --no-docs --use-vanilla fpcFeatures_0.0.0.0001.tar.gz

