# OpenTransportation - Concept

Similar to [OpenAddresses](https://openaddresses.io/) except for Transporation related datasets.

The hardest struggle when dealing with large volumes of data is consistency, having common data formats & attributes across all your datasets is the first steps of transportation related analysis.

## Cities Available

- [ ] City of Ottawa (Ontario, Canada)
- [ ] City of Toronto (Ontario, Canada)

## Core Services:

- All data hosted as Amazon S3 buckets
- Formatted into GeoJSON & Vector Tiles (phase 2)
- Pre-processed data based on OSM's highway scheme
- Historical data (current bucket will be the latest, past uploads will have timestamps with uploaded dates - used to for historical change analysis)

## Data Attributes

All data must follow the [OSM Highway scheme](https://wiki.openstreetmap.org/wiki/Key:highway).

- [`highway`](https://wiki.openstreetmap.org/wiki/Key:highway) (`residential`/`trunk`/`secondary`)
- [`lanes`](https://wiki.openstreetmap.org/wiki/Key:lanes) (`1`/`2`/`3`)
- [`maxspeed`](https://wiki.openstreetmap.org/wiki/Key:maxspeed) (`40`/`50 mph`)
- [`name`](https://wiki.openstreetmap.org/wiki/Key:name) (main name for the road - Value must conform to OSM naming convention)
- [`name:en` & `name:fr`](https://wiki.openstreetmap.org/wiki/Key:name) (or any other multilingual tags)
- [`surface`](https://wiki.openstreetmap.org/wiki/Key:surface) (`paved`/`unpaved`/`asphalt`)
- [`lit`](https://wiki.openstreetmap.org/wiki/Key:lit) (`yes`/`no`)

## Resources

- [Centerline Data Sources](https://github.com/osmlab/centerlines)
- [OSM QA Tiles](https://osmlab.github.io/osm-qa-tiles/)
- [Tippecanoe](https://github.com/mapbox/tippecanoe)
- [Tile Reduce](https://github.com/mapbox/tile-reduce)
- [TIGER Tiles](https://github.com/iandees/tiger-tiles)
- [TIGER Battlegrid](https://github.com/iandees/tiger-battlegrid)
- [SharedStreets](https://docs.google.com/document/d/1PsxUMWYniN3sKT0IbqC0RRC5nK9cno8P2BKk_MPn6t8/edit#heading=h.fltegbaf948o)
