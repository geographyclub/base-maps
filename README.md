# base-maps

My library of ready-to-use base maps.

Hillshade rasters made by combining elevation and hydrobasins.

Svg files of popular geographic datasets.

## Downloads

Browse files by category:

[Hillshade](https://github.com/geographyclub/base-maps/tree/main/hillshade/)

[Hillshade Color](https://github.com/geographyclub/base-maps/tree/main/hillshade_color/)

[Svg](https://github.com/geographyclub/base-maps/tree/main/svg/)

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
