The CMCC-ESM2 extractor works for netCDF files as published by Lovato et al (2022).
You can download their model outputs/nc files from the following link:
https://esgf-metagrid.cloud.dkrz.de/search
The NetCDF files can be directly downloaded from this online portal of Earth System Grid Foundation (ESGF).
You do have the option to download it using wget scripts, globus, openDAP etc.

For more information on the CMCC-ESM2 datasets, please check out their publication: 
CMIP6 Simulations With the CMCC Earth System Model (CMCC-ESM2)
https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021MS002814

The Data Extractor contains scripts for 3 kinds of data extractions:
1. Point location based: You can input your locations' coordinates. See the pointxy.csv file to identify the format
in which the data was input for point-location based extraction.
2. Domain based: You can input your domain vertices as coordinates. See the domainxy.csv file to identify the format
in which the data was input for the domain-based extraction.
3. Shapefile based: This is an extra snippet added later on to the extractor. A demo shapefile is added in the folder 
to test out usage. There is a csv file named 'merged_region_interest_pr_3hr_historical.csv' which contains the data 
extracted using the shapefile-based snippet. 

Please ensure the filepaths are based on your own directories.

The Xtractor is hardcoded for 'Amon' and 'Omon' datasets of CMCC-ESM2 by Lovato et al (2022). In case the variables 
you are using are of different dimensions, the names are in different format, you use not only the ssp126 or ssp585 
but other scenarios, ensure you correct/modify these parts in the code you download to use. A quick overview can 
be seen through the MetaData of the netcdf file you are using. Parts of the code may have to be modified based on 
the dataset/nc files you are using.