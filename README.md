# drought_za

South Africa drought analysis and prediction project using CHIRPS-derived drought indicators.

## Repository Contents

```text
drought_za/
|-- assets/
|   `-- images/
|       `-- drought_risk_map.png
|-- data/
|   `-- raw/
|       |-- assa-climate-data-district-annual-drought-2011-2025-chirps.csv
|       |-- assa-climate-data-national-annual-drought-2011-2025-chirps.csv
|       |-- assa-climate-data-provincial-annual-drought-2011-2025-chirps.csv
|       `-- sa_provinces.geojson
|-- notebooks/
|   |-- archive/
|   |   `-- Province_Drought_Risk_Analysis.executed.ipynb
|   |-- Drought_Prediction.ipynb
|   `-- Province_Drought_Risk_Analysis.ipynb
|-- .gitignore
|-- requirements.txt
`-- README.md
```

## Requirements

- Python 3.10+
- `pip` or `conda`
- Jupyter Notebook / JupyterLab

Install dependencies:

```bash
pip install -r requirements.txt
```

## Quick Start

1. Clone the repository.
2. Install dependencies from `requirements.txt`.
3. Open Jupyter:

```bash
jupyter notebook
```

4. Run notebooks from the `notebooks/` directory.

## Data Notes

- Notebooks are configured to load input data from `../data/raw/` (relative to `notebooks/`).
- `Drought_Prediction.ipynb` expects this additional file:
  - `data/raw/assa-climate-data-national-monthly-drought-2010-11-30_2025-11-01-chirps.csv`
- If that monthly file is not present, cells that use it will fail until added.

## Suggested Git Push Workflow

```bash
git init
git branch -M main
git remote add origin https://github.com/rabeshi/drought_za.git
git add .
git commit -m "Organize project structure, add README and requirements"
git push -u origin main
```
