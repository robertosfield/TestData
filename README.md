# TestData
Test data for OSG and VSG feature and performance testing

## Earth_VSG
The Earth_VSG directory contains a paged database that was created using a combination of [VirtualPlanetBuilder](https://github.com/openscenegraph/VirtualPlanetBuilder) and [vsgXchange](https://github.com/vsg-dev/vsgXchange), vsgXchange must be built with OpenSceneGraph dev installed in order to do the .osgb to .vsgb conversion :

    osgdem --geocentric --bluemarble-east -t BlueMarble/land_shallow_topo_east.tif --bluemarble-west -t BlueMarble/land_shallow_topo_west.tif -o Earth_OSG/earth.osgb

    vsgconv Earth_OSG/earth.osgb Earth_VSG/earth.vsgb -l 30

To view the database:

    vsgviewer Earth_VSG/earth.vsgb

