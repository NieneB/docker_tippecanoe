
## What is TippeCanoe? 

Developed by Mapbox. 
Builds vector tilesets from large (or small) collections of GeoJSON features.

https://github.com/mapbox/tippecanoe

This docker installs TippeCanoe in a docker container with command `TippeCanoe` so you can use docker to run the TippeCanoe commands.

How to build:

	docker build -t niene/tippecanoe .

To run the tippecanoe help :

	docker run --rm niene/tippecanoe --help

To run tippecanoe with options:

	docker run --rm -v `pwd`/data_tiles:/data_tiles niene/tippecanoe  -o out.mbtiles [and other tippecanoe commands]

	docker run --rm -v `pwd`/data_tiles:/data_tiles niene/tippecanoe  -o data_tiles/test.mbtiles /data_tiles/bgt_pand.geojson  

