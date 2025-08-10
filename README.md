# Danone ESG–SCM Case Study

## Project Overview
This project models the cradle-to-retail carbon footprint of a selected Danone product SKU (Yogurt, France, 2020 baseline), and identifies actionable levers to reduce emissions while aligning with ESG targets. The analysis applies **GHG Protocol Scope 1/2/3 accounting**, AGRIBALYSE LCIs, and scenario-based abatement cost modeling.

**Deliverables**:
- McKinsey-style presentation (10–12 slides)
- One-page KPI PDF (before/after)
- Reproducible Jupyter notebooks
- Documented assumptions and data sources

## Repo Structure
- `data/`: raw, processed datasets, and emission factors
- `notebooks/`: sequential analysis notebooks
- `src/`: reusable functions and modules
- `reports/`: final deliverables
- `docs/`: methodology, assumptions, and sources

## Getting Started
```bash
# clone repo
git clone https://github.com/YOURUSERNAME/danone-esg-case-study.git
cd danone-esg-case-study

# create virtual environment
python -m venv .venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows

# install requirements
pip install -r requirements.txt
