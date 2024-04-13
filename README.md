# base-maps
Color hillshade rasters made by combining elevation and hydrobasins -- georeferenced for developers.

## Downloads

Browse files here:

[Main directory](https://github.com/geographyclub/base-maps/tree/main/hillshade/)

## For Developers

Each png file has an accompanying pgw world file with information on the latlong coordinate system and extent of the raster. Open the png in any GIS software or use gdal to access these features.  

For example, to reproject a raster with gdal:  
```shell
gdalwarp -s_srs 'EPSG:4326' -t_srs <target_srs> nairobi-kenya.png nairobi-kenya.tif
```

## Data Sources

[HydroATLAS](https://www.hydrosheds.org/hydroatlas)

[Natural Earth](https://www.naturalearthdata.com/downloads/)

[SRTM Topography](https://catalog.data.gov/dataset/srtm15_plus-estimated-topography-15-seconds-global-v1)

[WWF Ecoregions](https://www.worldwildlife.org/publications/terrestrial-ecoregions-of-the-world)
