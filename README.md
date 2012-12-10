thailand.json
=============
I am working on D3.js project with map. 
I coudn't find GeoJson file for Thailand so I create one.

Using GDAL ogr2ogr convert shapefile(ESRI) to Geojson.

/Library/Frameworks/GDAL.framework/Versions/1.9/Programs/ogr2ogr -f "GeoJSON" -lco COORDINATE_PRECISION=6 thailand.json input.shp


Thailand GeoJson file.