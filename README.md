# TIA Files — Academic Integrative Project (TIA)

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-4-5B4638?logo=Python&logoColor=white)

An integrative university project (TIA — Trabalho Integrado Acadêmico) featuring a Jupyter Notebook that queries Brazilian municipal open data via the **Portal da Transparência API** and processes multiple CSV datasets for analysis.

> **Note:** This repository is a duplicate/sibling of `IA_FILES`. See that repo for a more detailed description.

## Features

- **API Client** — queries 8 categories of municipal data from `dadosabertos-portalfacil.azurewebsites.net`
- **Paginated Data Retrieval** — auto-pagination across API pages to build DataFrames
- **Data Categories:** Organizational, Contracts/Bidding, Budgetary, COVID-19, HR, Legislation, Public Works, Legislative Processes
- **Job Title Normalization** — `transmutar_lista_cargos()` using multi-stage regex
- **CSV Datasets Included:**
  - `servidores.csv` — Employee payroll (16 columns)
  - `biblia.csv` — Bible-related data
  - `dados_TIA_multidisciplinar.csv` — Multi-subject student assessment
  - `marketing_campaign.csv` — Marketing campaign analytics
  - `sao-paulo-properties-april-2019.csv` — SP property listings

## Tech Stack

Python, Jupyter Notebook/Google Colab, Pandas, Requests, BeautifulSoup, re

## Architecture

Single Jupyter Notebook (`Projeto_Integrador.ipynb`) with:
- API interaction functions (`categorias`, `loop_lista`, `busca_dados`, `make_df`)
- Data cleaning pipeline (`transmutar_lista_cargos`)
- Supplementary CSV datasets for analysis

## Usage

Open `Projeto_Integrador.ipynb` in Google Colab and run all cells.
