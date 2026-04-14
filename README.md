# Diurnal-cycle-choi-2026

## Diurnal Cycle of Precipitation: Evaluation of Satellite and Reanalysis Products

Code repository for:

> Choi, G. (2026). . Hydrology and Earth System Sciences.

### Overview

This repository contains Python code to reproduce all figures in the above manuscript.
The study evaluates the diurnal cycle of precipitation across satellite products
(IMERG, TRMM, CMORPH, GSMaP, MSWEP) and reanalysis datasets (ERA5, JRA-3Q, MERRA-2)
against ground-based observations (GSDR, HadISD, DWD, ECCC, KMA, CMFD).

### Requirements

- Python 3.9
- numpy, xarray, pandas, scipy
- matplotlib, cartopy, cmocean
- xesmf, xskillscore, mpltern

Install dependencies:
```bash
conda env create -f environment.yml
conda activate kite

Usage

1. Set data paths in the first cell of total_fig_code_submission.ipynb:

DATA_DIR = '/path/to/data'
FIG_DIR  = '/path/to/figures'

2. Run cells corresponding to each figure section.

Figures

┌─────────┬───────────────────────────────────────────────┐
│ Section │                  Description                  │
├─────────┼───────────────────────────────────────────────┤
│ 1       │ Observation station map                       │
├─────────┼───────────────────────────────────────────────┤
│ 2       │ Relative contributions of harmonic amplitudes │
├─────────┼───────────────────────────────────────────────┤
│ 3       │ Harmonic disagreement                         │
├─────────┼───────────────────────────────────────────────┤
│ 4       │ Harmonic phase and amplitude                  │
├─────────┼───────────────────────────────────────────────┤
│ 5       │ Global evaluation (bias)                      │
├─────────┼───────────────────────────────────────────────┤
│ 6       │ Precipitation type classification             │
├─────────┼───────────────────────────────────────────────┤
│ 7       │ IGRA SGP station vertical analysis            │
├─────────┼───────────────────────────────────────────────┤
│ 8       │ Vertical profiles from reanalysis             │
└─────────┴───────────────────────────────────────────────┘

Data Availability

Input data are available from:
- IMERG: NASA GES DISC
- ERA5: Copernicus Climate Data Store

Author

Gychoi — Pukyona National University  
