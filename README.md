# Offline Maps with MapsForge

* Used tools
  * [MapsForge](https://github.com/mapsforge/mapsforge) The library that parses the map file, handles and display the map.
  * [MapsForme MapWriter Plugin] (https://github.com/mapsforge/mapsforge/blob/master/docs/Downloads.md) This is needed if you want the library to handle a previously downloaded map to handle it offline.
    * Copy the downloaded plugin to 
      * Linux: `$USER_HOME/.openstreetmap/osmosis/plugins`
      * Windows `Application Data\Openstreetmap\Osmosis\Plugins` 
  * [Open Street Map] (https://www.openstreetmap.org/export) 
    * Use this service to download the region you want to be transformed by Osmosis from **pbf** to **map**
  * [Osmosis](http://wiki.openstreetmap.org/wiki/Osmosis)
    * Installation:
      * Linux:  <br/>
        `wget http://bretth.dev.openstreetmap.org/osmosis-build/osmosis-latest.tgz` <br/>
        `tar xvfz osmosis-latest.tgz -C osmosis` <br/>
        `rm osmosis-latest.tgz` <br/>
        `cd osmosis` <br/>
        `chmod a+x bin/osmosis` <br/>
        `bin/osmosis` <br/>
      * [Windows] (http://wiki.openstreetmap.org/wiki/Osmosis/Quick_Install_(Windows))
    * Usage:
      * Write map file for _city_ using Binary-PBF format and writing into file /tmp/_city_.map: <br/>
      `$ bin/osmosis --rb file=../data/city.osm.pbf --mapfile-writer file=/tmp/city.map`
* Code example
  * Coming soon
