# Osmosis-0.43
Correct Osmosis configuration for converting OSM files to MAP.

Steps for installation:

1. Move the all files downloaded to /opt directory

2. From root user
```
   1. $ export OSMOSIS_HOME=/opt/osmosis-0.43
   2. $ export PATH=$PATH:$OSMOSIS_HOME/bin
   3. $ echo "org.openstreetmap.osmosis.plugin.elasticsearch.ElasticSearchWriterPluginLoader" > $OSMOSIS_HOME/config/osmosis-plugins.conf
```
3. From local user
```
   1. $ export OSMOSIS_HOME=/opt/osmosis-0.43
   2. $ export PATH=$PATH:$OSMOSIS_HOME/bin
```

## Example for Convert OSM file to MAP

```
$ osmosis --read-xml <fileinput>.osm --mapfile-writer <fileoutput>.map
```


Please, visit the original source code: https://github.com/mapsforge/mapsforge

This small tutorial is based in the steps for [Convert from OpenStreetMap to Mapsforge using Osmosis](http://developer.servalproject.org/dokuwiki/doku.php?id=content:servalmaps:osmosis)

Others sites that was help:
* https://oss.sonatype.org/content/repositories/snapshots/org/mapsforge/mapsforge-map-writer/
* http://download.geofabrik.de/
* http://wiki.openstreetmap.org/wiki/Osmosis/Installation#Linux
* http://wiki.openstreetmap.org/wiki/Converting_map_data_between_formats
