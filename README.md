# pacea_bathymetry
 Code to add bathymetry data to the pacea grid.

 Bathymetry data comes from Gebco gridded global bathymetry data. British Oceanographic Data Centre, (https://www.gebco.net/) using the GEBCO 2023 grid, from -146W to -117E , and 42S to 58N, downloaded as a netcdf.

 Data was reprojected into BC albers coordinate reference system, EPSG:3005, and resampled onto a grid of 500x500m resolution, to the extent of the base grid (grid 26) in the pacea package.

 Zonal statistics were then completed using the exactextractr package, to calculate the mean, max, and minimum depth values in each cell of the pacea grid.
