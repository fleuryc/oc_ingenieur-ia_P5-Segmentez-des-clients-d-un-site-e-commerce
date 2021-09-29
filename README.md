[![Python application](https://github.com/fleuryc/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/actions/workflows/python-app.yml/badge.svg)](https://github.com/fleuryc/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/actions/workflows/python-app.yml)
[![CodeQL](https://github.com/fleuryc/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/fleuryc/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/actions/workflows/codeql-analysis.yml)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/acbad042d6594e0d88a3443d573d3dfd)](https://www.codacy.com/gh/fleuryc/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/dashboard)
[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/acbad042d6594e0d88a3443d573d3dfd)](https://www.codacy.com/gh/fleuryc/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/dashboard)

- [Olist : Categorize clients for a e-commerce website](#olist--categorize-clients-for-a-e-commerce-website)
  - [Installation](#installation)
    - [Prerequisites](#prerequisites)
    - [Virtual environment](#virtual-environment)
    - [Dependencies](#dependencies)
  - [Usage](#usage)
    - [Run Notebook](#run-notebook)
    - [Quality Assurance](#quality-assurance)
  - [Troubleshooting](#troubleshooting)

* * *

# Olist : Categorize clients for a e-commerce website

Repository of OpenClassrooms' [AI Engineer path](https://openclassrooms.com/fr/paths/188-ingenieur-ia), project #5

Goal : use Jupyter Notebook and Scikit-Learn to create, assess and improve a clustering model based on customers and orders data.

You can see the results here :

-   [Presentation](https://fleuryc.github.io/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/index.html)

-   [HTML page with interactive plots](https://fleuryc.github.io/oc_ingenieur-ia_P5-Segmentez-des-clients-d-un-site-e-commerce/notebook.html)

## Installation

### Prerequisites

-   [Python 3.9](https://www.python.org/downloads/)

### Virtual environment

```bash
make venv
source env/bin/activate
```

### Dependencies

```bash
# pip install kaggle jupyterlab ipywidgets numpy pandas
# > or :
# pip install -r requirements.txt
# > or :
make install
```

## Usage

### Run Notebook

```bash
jupyter-lab notebooks/main.ipynb
```

### Quality Assurance

```bash
# make isort
# make format
# make lint
# make bandit
# make mypy
# make test
# > or just :
make qa
```

## Troubleshooting

-   Fix Plotly issues with JupyterLab

cf. [Plotly troubleshooting](https://plotly.com/python/troubleshooting/#jupyterlab-problems)

```bash
jupyter labextension install jupyterlab-plotly
```

-   If using Jupyter Notebook instead of JupyterLab, uncomment the following lines in the notebook

```python
import plotly.io as pio
pio.renderers.default='notebook'
```
