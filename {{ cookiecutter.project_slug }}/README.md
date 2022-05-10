# {{ cookiecutter.project_name }} 

By: {{ cookiecutter.project_author_name }}.

Version: {{ cookiecutter.project_version }}

{{ cookiecutter.project_description }}

## Prerequisites

- [Anaconda](https://www.anaconda.com/download/) >=4.x
- Optional [Mamba](https://mamba.readthedocs.io/en/latest/)

## Create environment

```bash
conda env create -f environment.yml
activate {{ cookiecutter.project_slug }}
```

or 

```bash
mamba env create -f environment.yml
activate {{ cookiecutter.project_slug }}
```

## Project organization

    {{ cookiecutter.project_slug }}
        ├── data
        │   ├── processed      <- The final, canonical data sets for modeling.
        │   └── raw            <- The original, immutable data dump.
        │
        ├── model              <- Save the model
        |
        ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
        │                         the creator's initials, and a short `-` delimited description, e.g.
        │                         `1.0-initial-data-exploration`.
        ├── src                <- Scripts for the preparation and training of the model.
        |
        ├── utilities          <- Useful functions that could help us.
        |
        ├── .gitignore         <- Files to ignore by `git`.
        │
        ├── environment.yml    <- The requirements file for reproducing the analysis environment.
        │
        └── README.md          <- The top-level README for developers using this project.
---