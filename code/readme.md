#  Bayesian Reaction Optimization as A Tool for Chemical Synthesis

In this capsule we provide example code for Bayesian reaction optimization which can be used to explore some of our software’s features and reproduce simulation results presented in the corresponding paper.

## Software

Experimental Design via Bayesian Optimization: *edbo* is a practical python implementation of Bayesian optimization. Documentation for the main modules can be found on the documentation page or by using help(edbo.module).

**Documentation:** https://b-shields.github.io/edbo/index.html

## Installation

(0) Create anaconda environment

```
conda create --name edbo python=3.7.5
```

(1) Install rdkit, Mordred, and PyTorch

```
conda activate edbo
conda install -c rdkit rdkit
conda install -c rdkit -c mordred-descriptor mordred
conda install -c pytorch pytorch=1.3.1
```

(2) Install EDBO

```
pip install edbo
```

### Running Notebooks

```
conda install jupyterlab
```

### GPU Integration

```
conda install cudatookit=10.1, torchvision -c pytorch
```