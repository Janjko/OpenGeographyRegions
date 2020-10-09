# OpenGeographyRegions
A project to create a free, global, crowdsourced, multilingual dataset of geographic regions. This is work in progress, pull requests and other input are welcome. 

## Simple polygons, appropriate for different scales.
Starting with [natural earths](https://www.naturalearthdata.com/) 10m geography dataset.

## Linked Data (permits internationalization and semantics through integration with other datasets)
Add a property "wikidata" with value "Q23" to reference a wikidata object.

## Open License
The license is CC0.

## Data in GeoJSON
The data is available in GeoJSON. 
Currently used feature classes (and usage count), derived from natural earth:

### geography_10m.geojson
* 165 "archipel"
*   9 "basin"
*  37 "coast"
*   7 "continent"
*  12 "delta"
*   2 "depression"
*  58 "desert"
*   3 "foothills"
*  44 "geoarea"
*   3 "gorge"
* 295 "island"
*   4 "isthmus"
*   3 "lake"
*   5 "lowland"
* 222 "mountain_range"
*  68 "peninsula"
*  30 "plain"
*  72 "plateau"
*   4 "tundra"
*   6 "valley"
*   3 "wetlands"

The statistics are printed quick + dirty with this bash line: `cat geography_10m.geojson |cut -f 9 -d" "|sort|uniq -c`
