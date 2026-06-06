# Indonesia Import Analysis

A data analysis project exploring global product trends and import opportunities for Indonesia.

## Overview

This project combines Google Trends data (via `pytrends`) with UN Comtrade trade statistics (via `comtradeapicall`) to identify high-demand global products that present import opportunities for Indonesia. The goal is to surface actionable insights for traders, policymakers, and market researchers.

## Project Structure

```
indonesia-import-analysis/
├── data/
│   ├── raw/          # Raw data downloaded from APIs (Comtrade, Google Trends)
│   └── processed/    # Cleaned and merged datasets ready for analysis
├── output/
│   ├── charts/       # Generated visualizations (PNG, SVG)
│   └── csv/          # Exported result tables
├── src/              # Python scripts for data collection and analysis
├── notebooks/        # Jupyter notebooks for exploration and reporting
├── requirements.txt
└── .gitignore
```

## Data Sources

- **Google Trends** — global search interest by product/keyword via `pytrends`
- **UN Comtrade** — Indonesia import/export volumes and trade values via `comtradeapicall`

## Setup

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Usage

1. Place API credentials in a `.env` file (not committed — see `.gitignore`)
2. Run data collection scripts in `src/` or explore via notebooks in `notebooks/`
3. Outputs are written to `output/charts/` and `output/csv/`
