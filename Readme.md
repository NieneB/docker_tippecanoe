
## TippeCanoe 

Tippecanoe is developed by Mapbox. It builds vector tilesets from large (or small) collections of GeoJSON features.
For original source and commands see: https://github.com/mapbox/tippecanoe

This docker installs TippeCanoe in a docker container with entrypoint  `tippecanoe` so you can use docker to run the TippeCanoe command.

How to build:

	docker build -t niene/tippecanoe .

To run the tippecanoe help :

	docker run --rm niene/tippecanoe --help

To run tippecanoe with options:

	docker run --rm -v `pwd`/data_tiles:/data_tiles niene/tippecanoe  -o out.mbtiles [and other tippecanoe commands]

	docker run --rm -v `pwd`/data_tiles:/data_tiles niene/tippecanoe  -o data_tiles/test.mbtiles /data_tiles/test.geojson 

See https://github.com/mapbox/tippecanoe for all the TippeCanoe options!  

