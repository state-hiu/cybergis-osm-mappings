CyberGIS OSM Mappings (cybergis-osm-mappings)
================

## Description

This repository contains OpenStreetmap (OSM) mappings for use by GeoGig.  See the "Using GeoGig with OpenStreetMap Data" page for more information at: [http://geogig.org/docs/interaction/osm.html](http://geogig.org/docs/interaction/osm.html).  The mappings folder includes the mappings in json format.  The mappings are broken out into namespaces/categories, mostly following ISO categories.  These are standardized mappings that should represent most basic OSM features, but also cover common mispellings and mistaggings.

See the guides in the cybergis-guides repo at [https://github.com/state-hiu/cybergis-guides/](https://github.com/state-hiu/cybergis-guides), for examples on use these mappings.

### CyberGIS
The Humanitarian Information Unit has been developing a sophisticated geographic computing infrastructure referred to as the CyberGIS. The CyberGIS provides highly available, scalable, reliable, and timely geospatial services capable of supporting multiple concurrent projects.  The CyberGIS relies on primarily open source projects, such as PostGIS, GeoServer, GDAL, GeoGit, OGR, and OpenLayers.  The name CyberGIS is dervied from the term geospatial cyberinfrastructure.

### ROGUE
The Rapid Opensource Geospatial User-Driven Enterprise (ROGUE) Joint Capabilities Technology Demonstration (JCTD) is a two-year research & development project developing the technology for distributed geographic data creation and synchronization in a disconnected environement.  This new technology taken altogether is referred to as GeoSHAPE.  See [http://geoshape.org](http://geoshape.org) for more information.  HIU is leveraging the technology developed through ROGUE to build out the CyberGIS into a robust globally distributed infrastruture.

## Installation

These installation instructions are subject to change.  Right now, since there are no debian package dependencies, you can really extract the repo to whatever directory you want.  The instructions below are suggested as they mirror Linux best practices for external packages.

As root, execute the following commands:
```
cd /opt
git clone https://github.com/state-hiu/cybergis-osm-mappings.git cybergis-osm-mappings.git
```

The CyberGIS Scripts repo (cybergis-scripts) also contains some tools for automating the process of creating OpenStreetMap extracts.  See the installation guide at [https://github.com/state-hiu/cybergis-scripts](https://github.com/state-hiu/cybergis-scripts).

## Usage

Extents are currently limited to bounding boxes in the `S W N E` format to conform closely to the `osm download` command explained in the [Downloading data from an OSM Server](http://geogig.org/docs/interaction/osm.html#downloading-data-from-an-osm-serve) section of the GeoGig User Manual.  Complex geometry extents are possible but are not sufficiently integrated to work at scale.  You can do complex geometry extents, but it currently requires hand writing filters using the [Overpass Query Language](http://wiki.openstreetmap.org/wiki/Overpass_API/Language_Guide).

The easist mapping to start with is the `basic:buildings_and_roads` mapping available at [[link]](https://github.com/state-hiu/cybergis-osm-mappings/blob/master/mappings/basic/buildings_and_roads.json).

You can learn more about OSM mappings from the GeoGig User Manual at [http://geogig.org/docs/interaction/osm.html#data-mapping](http://geogig.org/docs/interaction/osm.html#data-mapping).

To learn how to create extracts check out the OSM Extracts CyberGIS Guide at [[link]](https://github.com/state-hiu/cybergis-guides/blob/master/1.0/cybergis-guides-osmextracts-1.0.md).  You can also look at examples of extracts of [Khulna, Bangladesh](https://github.com/state-hiu/cybergis-scripts/tree/master/examples/khulna) and [Ebola Crisis](https://github.com/state-hiu/cybergis-scripts/tree/master/examples/ebola).

### Extents

Below is a list of extent namespaces.

1. [Bangladesh](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/extents/bangladesh)
2. [Dominican Republic](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/extents/dominican_republic)
3. [Honduras](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/extents/honduras)
4. [Liberia](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/extents/liberia)
5. [Sierra Leone](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/extents/sierra_leone)
6. [Turkey](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/extents/turkey)

### Mappings

Below is a list of mapping namespaces.

1.  [Basic](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/basic)
2.  [Education](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/education)
3.  [Health](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/health)
4.  [Inland Waters](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/inlandWaters)
5.  [Landuse](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/landuse)
6.  [Placenames](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/placenames)
6.  [Roads](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/roads)
7.  [Structure](https://github.com/state-hiu/cybergis-osm-mappings/tree/master/mappings/structure)

## Contributing

HIU is currently accepting pull requests for this repository.  Please provide a human-readable description of the mappings in the pull request.  Additionally, update the README.md file as needed.

## License
This project constitutes a work of the United States Government and is not subject to domestic copyright protection under 17 USC § 105.

However, because the project utilizes code licensed from contributors and other third parties, it therefore is licensed under the MIT License. http://opensource.org/licenses/mit-license.php. Under that license, permission is granted free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the conditions that any appropriate copyright notices and this permission notice are included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
