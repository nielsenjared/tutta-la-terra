# The Universal Description of the Whole Earth Known to Date

Mobile-friendly, interactive map created using:

* Library of Congress Digital Collection (https://www.loc.gov/resource/g3200.mf000070/)
* Leaflet (http://leafletjs.com/)
* leaflet-rastercoords (https://commenthol.github.io/leaflet-rastercoords/)
* gdal2tiles-leaflet (https://github.com/commenthol/gdal2tiles-leaflet)

## Check It Out

http://jarednielsen.com/tutta-la-terra/

Follow the Geography and Map Division of the Library of Congress on Twitter: https://twitter.com/LOCMaps

And watch #MapMonsterMonday: https://twitter.com/hashtag/MapMonsterMonday?src=hash


## DIY

Download or clone this repo.

Download the .tif file for this beast: https://www.loc.gov/resource/g3200.mf000070/

And copy or move it to this repo directory.

You need `gdal2tiles.py` to make tiles. Clone (or download) into the current directory:

`git clone https://github.com/commenthol/gdal2tiles-leaflet.git`

Change into it:

`cd gdal*`

And run:

`python gdal2tiles.py -l -p raster -z 0-6 -w none ./mf000070.tif ./tiles`

Voila! Open `map.html` in your browser.
