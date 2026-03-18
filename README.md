
# MSBD570 Final Project — Diabetes Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Repository Structure](#repository-structure)
- [Requirements & Setup](#requirements--setup)
- [Notebooks & Workflow](#notebooks--workflow)
- [Reproducibility](#reproducibility)
- [Outputs](#outputs)
- [Contributing](#contributing)
- [Contact](#contact)

## Project Overview

This repository contains the final project for MSBD570. The project performs data cleaning, exploratory data analysis, visualization, and (optionally) simple modeling on a diabetes dataset. The work is organized into Jupyter notebooks and supporting scripts/resources under `src`.

## Dataset

- Cleaned dataset: [data/cleaned_diabetes_data.csv](data/cleaned_diabetes_data.csv)

Brief description: the cleaned dataset contains patient-level features relevant to diabetes analysis (see notebooks for a full variable description and preprocessing steps).


## Repository Structure

- [data](data) — datasets used in this project
- [notebooks](notebooks) — Jupyter notebooks used for loading, EDA, and visualization
	- [notebooks/01_data_loading.ipynb](notebooks/01_data_loading.ipynb)
	- [notebooks/02_eda.ipynb](notebooks/02_eda.ipynb)
	- [notebooks/03_visualizations.ipynb](notebooks/03_visualizations.ipynb)
- [outputs](outputs) — exported figures, tables, and other artifacts
- [requirements.txt](requirements.txt) — Python dependencies

## Requirements & Setup

Recommended Python version: 3.8+ (use virtualenv/venv or conda).

Install dependencies:

```bash
python3 -m pip install -r requirements.txt
```

Run JupyterLab or Jupyter Notebook to open and run the notebooks:

```bash
jupyter lab
# or
jupyter notebook
```

## Notebooks & Workflow

High-level workflow (follow this order):

1. `notebooks/01_data_loading.ipynb` — load dataset and perform initial cleaning, save the cleaned CSV to `data/`.
2. `notebooks/02_eda.ipynb` — exploratory data analysis, summary statistics, and feature inspection.
3. `notebooks/03_visualizations.ipynb` — generate figures and visualizations; saved outputs appear under `outputs/`.

Each notebook contains narrative cells explaining the steps, and code cells you can re-run end-to-end.

## Reproducibility

- Use the provided `requirements.txt` to create a consistent environment.
- Notebooks set random seeds where modeling is performed; if you add new randomized steps, set seeds explicitly.
- To reproduce results: install deps, open notebooks in order, and run all cells.

## Outputs

Generated artifacts (figures, tables) are saved to the `outputs/` directory. Inspect that folder after running the visualization notebook.

## Contributing

If you want to extend this project:

- Add new notebooks or scripts under `notebooks`.
- Update `requirements.txt` if you add new Python packages.
- Open an issue or send a pull request with proposed changes.

---



