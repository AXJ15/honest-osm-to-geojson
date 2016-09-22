# honest-osmtogeojson
honest-osmtogeojson is a python package that converts OSM data represented in (XML format) into a GeoJSON data represented in (JSON), inspired by the JavaScript module [osmtogeojson](https://github.com/tyrasd/osmtogeojson).

Top Features:

* under-development
* real OSM [polygon detection](https://wiki.openstreetmap.org/wiki/Overpass_turbo/Polygon_Features)
* can convert the entire OSM data in one go << this's the actualy reason behind building this package :)
* works with extra large data 100 MB, 1 GB, 10GB, or 50GB, without exhausting the computer resources

Differences from the JavaScript module [osmtogeojson](https://github.com/tyrasd/osmtogeojson):

* server-sided usage only, this is a python package it won't work on browser :).
* GeoJSON feature's flat properties by convention, it will be simply a list of key-value pairs instead of the unnecessary structured JSON object overhead.
* a whole different algorithm to process the anomalies of converting OSM data into GeoJSON data, this package will try to avoid duplicated data as much as possible, I'll go through this further in the follow up sections.

# Installation
to install this package, simply execute the following terminal command:

