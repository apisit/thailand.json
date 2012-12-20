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


The MIT License (MIT)
Copyright (c) 2012 Apisit Toompakdee

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
