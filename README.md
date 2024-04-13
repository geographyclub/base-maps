# base-maps
Colored hillshade rasters made for designers, georeferenced for developers.

## Downloads

Browse files here:

[Hillshade directory](https://github.com/geographyclub/base-maps/tree/main/hillshade/)

## For Developers

Each png file has an accompanying pgw world file with information on the latlong coordinate system and extent of the raster. Open the png in any GIS software or use gdal to access these features.  

For example, to reproject a raster with gdal:  
```shell
gdalwarp -s_srs 'EPSG:4326' -t_srs <target_srs> nairobi-kenya.png nairobi-kenya.tif
```
