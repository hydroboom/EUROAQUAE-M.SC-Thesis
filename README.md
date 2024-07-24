# Overview
Welcome to the repository for my thesis project, which is part of my Master's program at Warsaw University of Technology under the EUROAQUAE+ consortium. This project involves remote research in collaboration with Deltares, NL, and focuses a simple, generally usable methodology for selecting a representative years from single variables and multiple variables. The datasets used for developing the methodology are climate model outputs, from the following sources:

"Statistically downscaled CMIP6 ocean variables for European waters" by Kristiansen et al (2024):
Paper: https://www.nature.com/articles/s41598-024-51160-1
Dataset: https://zenodo.org/records/10794443

"CMIP6 Simulations With the CMCC Earth System Model (CMCC-ESM2)" by Lovato et al (2022):
Paper: https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021MS002814
Dataset: https://esgf-metagrid.cloud.dkrz.de/search

# Project Description
This repository contains all the files and code related to my research work. The thesis involves extensive data analysis and aims to provide a simple method for selecting representative year from a timeseries of climate model outputs. The following folders and codes are included in this repository:

1. Extractor for FUMA: contains a IPYNB script with readme file for extracting data from Kristiansen et al (2024) dataset.
  It also contains some demo outputs as csv files.
2. Extractor for CMCC-ESM2: contains a IPYNB script with readme file for extracting data from Lovato et al (2022) dataset.
  It also contains demo files for inputs (domainxy.csv, pointxy.csv, merged_region_interest.shp) and an output file (mergen_region_interest_pre_3hr_historical.csv)
3. FS Comparison: contains a IPYNB script with readme file and demo input csv files.
4. Correlation and PCA Script: contains a IPYNB with readme file, demo input and demo output for commonly used Correlation Matrix and Pripcipal Component Analysis.
5. SVM Script and Data: this is the folder for the script I wrote to select representative year (RY) from a single variable. The folder contains demo input files as csv and demo output files in folders, along with a readme file.
6. MVM Script and Data: this is the folder for the script I wrote to select a composite RY from multiple variables. The Folder contains demo input files (in folders) and a demo output folder ('Normalized') to be used in the script. More information available in the readme file within this forlder. 
