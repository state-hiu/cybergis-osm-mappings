CyberGIS OSM Mappings (cybergis-osm-mappings)
================

## Description

This repository contains OSM mappings for use by GeoGit.  See the "Using GeoGit wish OpenStreetMap Data" page for more information at: [http://geogit.org/docs/interaction/osm.html](http://geogit.org/docs/interaction/osm.html).  The mappings folder includes the mappings in json format.  The mappings are broken out into namespaces/categories, mostly following ISO categories.

See the guides in the cybergis-guides repo at [https://github.com/state-hiu/cybergis-guides/](https://github.com/state-hiu/cybergis-guides), for examples on use these mappings.

### CyberGIS
The Humanitarian Information Unit has been developing a sophisticated geographic computing infrastructure referred to as the CyberGIS. The CyberGIS provides highly available, scalable, reliable, and timely geospatial services capable of supporting multiple concurrent projects.  The CyberGIS relies on primarily open source projects, such as PostGIS, GeoServer, GDAL, GeoGit, OGR, and OpenLayers.  The name CyberGIS is dervied from the term geospatial cyberinfrastructure.

### ROGUE
The Rapid Opensource Geospatial User-Driven Enterprise (ROGUE) Joint Capabilities Technology Demonstration (JCTD) is a two-year research & development project developing the technology for distributed geographic data creation and synchronization in a disconnected environement.  See [http://rogue.lmnsolutions.com](http://rogue.lmnsolutions.com) for more information.  HIU is leveraging the technology developed through ROGUE to build out the CyberGIS into a robust globally distributed infrastruture.

## Installation

These installation instructions are subject to change.  Right now, since there are non-debian package dependencies, you can really extract the repo to whatever directory you want.  The instructions below are suggested as they mirror Linux best practices for external packages.

As root, execute the following commands:
```
cd /opt
git clone https://github.com/state-hiu/cybergis-osm-mappings.git cybergis-osm-mappings.git
```
Logout and Login

## Usage


## Contributing

HIU is currently accepting pull requests for this repository.  Please provide a human-readable description of the mappings in the pull request.

## License
This project constitutes a work of the United States Government and is not subject to domestic copyright protection under 17 USC § 105.

However, because the project utilizes code licensed from contributors and other third parties, it therefore is licensed under the MIT License. http://opensource.org/licenses/mit-license.php. Under that license, permission is granted free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the conditions that any appropriate copyright notices and this permission notice are included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
