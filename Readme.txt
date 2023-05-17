Python imports used:
numpy, pandas, matplotlib.pyplot, and scipy are used for statistics.
xarray and cartops.crs are used for mapping.
netCF4 is used for importing the sediment data.


Data downloads:

deep_sea_coral_sponge_data.csv: downloaded from the NOAA Deep Sea Coral and Sponge Map at https://www.ncei.noaa.gov/products/noaa-deep-sea-coral-and-sponge-map, with no modifications. Used in almost all of the created code.

seabed_lithology_v1.nc: downloaded from the GPlatesPortal Seafloor Lithology Map at https://portal.gplates.org/portal/seafloor/, with no modifications. Used in Preliminary_Sediment_Observation.ipynb, Sponge_Sediment_Distribution_(Incomplete).ipynb, and Sponge_Map.ipynb.


Created code:
maptools.py:
This file contains a function for making maps easier to create. 

Preliminary_Sponge_Analysis.ipynb:
This notebook contains the initial analysis of the dataset, including functions to sort out the sponge data from the coral data, to seperate the sponge data into classes, and to plot the sponge data relative to depth, latitude, and longitude. Requires the statistics imports.

Preliminary_Sediment_Observation.ipynb:
This notebook contains the initial look at the seafloor lithology dataset, including code for preparing the database for use, mapping the data, and determining what the values in the data mean. Requires the stats, mapping, and netCF4 imports.

Sponge_Map.ipynb:
This notebook contains mapping of the sponge and seafloor data, particularly comparing hexactinellids (glass sponges) and demosponges. Requires the stats, mapping, and netCF4 imports.

Sponge_Depth_Distribution.ipynb:
This notebook contains analysis of the distribution of sponges based on depth, particularly comparing hexactinellids (glass sponges) and demosponges. Requires the statistics imports.

Sponge_Latitude_Distribution.ipynb:
This notebook contains analysis of the distribution of sponges based on latitude, particularly comparing hexactinellids (glass sponges) and demosponges and with focus on the Northern Hemisphere. Requires the statistics imports.

Sponge_Sediment_Distribution_(Incomplete).ipynb:
This notebook begins coding for the analysis of the distribution of sponges based on seafloor lithology. Due to time the code would take to run, the analysis is incomplete. Requires the stats and netCF4 imports.