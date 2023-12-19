# hash:sha256:4f0ce03b6d2f5f6e1e639a72968cefe2bf7deb87928aa3e40b2cba52763342bb
FROM registry.codeocean.com/codeocean/miniconda3:4.8.2-python3.8-ubuntu18.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        libsm6=2:1.2.2-1 \
        libxext6=2:1.3.3-1 \
        libxrender1=1:0.9.10-1 \
    && rm -rf /var/lib/apt/lists/*

RUN conda install -y --channel=rdkit --channel=mordred-descriptor --channel=pytorch \
        dill==0.3.3 \
        jupyterlab==2.2.6 \
        matplotlib==3.3.2 \
        mordred==1.2.0 \
        numpy==1.17.4 \
        pandas==0.25.3 \
        python==3.7.5 \
        pytorch==1.3.1 \
        rdkit==2020.03.3.0 \
        scikit-learn==0.22.1 \
        seaborn==0.11.0 \
        statsmodels==0.12.1 \
        torchvision==0.4.2 \
        xlrd==1.2.0 \
    && conda clean -ya

RUN pip install -U --no-cache-dir \
    gpytorch==1.0.0 \
    pyclustering==0.9.3.1 \
    pyro-ppl==1.1.0 \
    pytest==6.1.2
