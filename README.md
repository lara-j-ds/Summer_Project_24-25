# Summer Project
Working in jupyter notebook for summer project of 24/25. Mainly using matplotlib, xarray and cartopy to graph atmospheric data  

To use files from fresh install of python will need to pip install notebook, numpy, scipy, xarray, matplotlib, cartopy, holoviews, hvplot, geoviews  

## File Guide
Xarray_StartupGuide --> The basics of xarray + some extras: how to load in and plot data, including with map projections, vectors, animation  
MakingPlots --> slightly more in depth than xarray guide, covers most plots useful for atmospheric data + some miscellaneous other types of graphs  
            --> also shows how to make interactive plots two different ways  
O3_Figures --> uses ozone data specifically, most helpful for scalar data focusing on concentration levels/chemistry based on location + pressure level  
Windfields --> uses wind data, most helpful for vector data based on location  
matplotlib, xarray --> not useful, just shows my first steps when learning how to use matplotlib and xarray  

## **Common error messages and solutions:**  

Download/SSL error when using cartopy; happens when required files can't be automatically downloaded, so have to download them manually.  
Fix: go to https://www.naturalearthdata.com/downloads/ or urls specified in error and download required files. Extract all files in user/.local/share/cartopy/shapefiles/natural_earth/physical (or cultural depending on the feature).

NetCDF/HDF error; dataset file is likely open somewhere else.  
Fix: restart the kernel in jupyter notebook (press 0 twice), then rerun required cells.  

SyntaxWarning: invalid escape sequence; likely used a / somewhere in a string.  
Fix: change / to either // or \, or change string assignment to r'whatever path is' to accept raw input
