# Pine White Butterfly Distribution  in BC

This repository contains spatial and ecological data used and the r code used for analyzing spatial distribution of Pine White butterfly in British Columbia, Canada. It includes processed datasets in `.csv` and `.Rda` formats, suitable for spatial modeling and visualization in R.

-----

## Data Files

| Filename                        | Description |
|--------------------------------|-------------|
| `BC_Covariates.Rda`            | R binary file containing spatial covariates such as elevation, forest cover, HFI (Human Footprint Index), and proximity to water. |
| `BC_Parks.Rda`                 | R binary file with the spatial location of provincial parks in British Columbia. |
| `clean_data_utm.csv`           | Cleaned dataset with spatial covariates and projected coordinates converted from WGS 84 (EPSG:4326) to BC Albers (EPSG:3005), used for spatial analysis. |
| `Neophasia_menapia_Canada.csv` | CSV file containing species observation records of *Neophasia menapia* in BC from Global Biodiversity Information Facility (GBIF). |

## Code Files

>Required R packages: `spatstat`, `sf`, `ks`

| Filename          | Description |
|-------------------|-------------|
| `data_preprocess.qmd` | Script for preprocessing data, including the conversion of projected coordinates from WGS 84 (EPSG:4326) to BC Albers (EPSG:3005).|
| `analysis.qmd`   | Main script for conducting spatial analysis using covariate data. |
| `analysis_output.html`   | Rendered HTML report containing both the analysis code and output visualizations/results. |