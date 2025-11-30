# Module8_ENSO_SMYLE
# ENSO Prediction Skill Using CESM2-SMYLE  
### ATMS 523 – Module 8 Project  
Author: Yudi Mao  

## Overview
This project evaluates the short-lead prediction skill of ENSO using the CESM2-SMYLE decadal prediction system.  
Niño-3.4 SST anomalies are computed, and skill is assessed using the Anomaly Correlation Coefficient (ACC) and Root-Mean-Square Error (RMSE).  
This notebook demonstrates an end-to-end reproducible workflow using Python and the tools taught in ATMS 523.

## Data
CESM2-SMYLE hindcast system  
Yeager et al. (2022), *Journal of Advances in Modeling Earth Systems*  
DOI: https://doi.org/10.1029/2021MS002529  

Variable: near-surface ocean temperature (SST, `tos`)  
Region: Niño-3.4 (5°S–5°N, 170°W–120°W)  
Leads: 0–12 months  

## Contents
- **fig1_RMSE_corr_multi_ens_Module8.ipynb** — main analysis notebook  
- **README.md** — project description  

## Workflow
1. Load CESM2-SMYLE SST data with `xarray`  
2. Compute Niño-3.4 index and anomalies  
3. Calculate ACC and RMSE vs. forecast lead  
4. Visualize ENSO skill characteristics  

## Results
- ACC is highest at short leads and decreases with lead time  
- RMSE increases with lead, indicating forecast error growth  
- Patterns are consistent with known ENSO predictability behavior  

## Reproducibility
Run the notebook in any Python environment with:  
`xarray`, `numpy`, `matplotlib`, `netCDF4`

