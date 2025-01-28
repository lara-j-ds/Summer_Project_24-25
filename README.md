# Summer Project
Working in jupyter notebook for summer project of 24/25. Mainly using matplotlib, xarray and cartopy to graph atmospheric data  

To use files from fresh install of python will need to pip install notebook, numpy, scipy, xarray, matplotlib, cartopy, holoviews, hvplot, geoviews  
   
   
**Common error messages and solutions:**  

Download/SSL error when using cartopy; happens when required files can't be automatically downloaded, so have to download them manually.  
Fix: go to https://www.naturalearthdata.com/downloads/ or urls specified in error and download required files. Extract all files in user/.local/share/cartopy/shapefiles/natural_earth/physical (or cultural depending on the feature).

NetCDF/HDF error; dataset file is likely open somewhere else.  
Fix: restart the kernel in jupyter notebook (press 0 twice), then rerun required cells. 
