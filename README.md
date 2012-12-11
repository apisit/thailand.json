thailand.json
=============
I am working on D3.js project with map. 
I coudn't find GeoJson file for Thailand so I create one.

Using GDAL ogr2ogr convert shapefile(ESRI) to Geojson.

/Library/Frameworks/GDAL.framework/Versions/1.9/Programs/ogr2ogr -f "GeoJSON" -lco COORDINATE_PRECISION=6 thailand.json input.shp


*Select field

/Library/Frameworks/GDAL.framework/Versions/1.9/Programs/ogr2ogr -select "CHA_NE" -f "GeoJSON" -lco COORDINATE_PRECISION=6 thailand.json gi_changwatv7308.shp 

Thailand GeoJson file.