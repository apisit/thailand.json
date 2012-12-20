thailand.json
=============
I am working on my personal project using D3.js and I want to display the map of Thailand.

I coudn't find GeoJson file for Thailand so I created one.

Using GDAL ogr2ogr convert shapefile(ESRI) to Geojson.

/Library/Frameworks/GDAL.framework/Versions/1.9/Programs/ogr2ogr -f "GeoJSON" -lco COORDINATE_PRECISION=6 thailand.json input.shp



How to select only one field to your output.
use -select "fieldname"

/Library/Frameworks/GDAL.framework/Versions/1.9/Programs/ogr2ogr -select "CHA_NE" -f "GeoJSON" -lco COORDINATE_PRECISION=6 thailand.json TH_shape/gi_changwatv7308.shp 


I also included simplified version of Thailand's Shapefile.

thailand.json is an output from shapefile. (301.394 kb)
thailandWithName.json is the simplified vector version. (162 kb)

