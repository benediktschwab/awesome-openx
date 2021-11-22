# Awesome OpenX [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

A curated list of awesome applications, libraries and datasets concerning the development and testing of automated driving functions with a focus on [ASAM OpenX Standards](https://www.asam.net/standards/) (e.g. [OpenDRIVE](https://www.asam.net/standards/detail/opendrive/), [OpenSCENARIO](https://www.asam.net/standards/detail/openscenario/), ...).

This is a list of [free](https://en.wikipedia.org/wiki/Free_software) software and datasets, whereas non-free software will be listed on the [non-free](non-free.md) page.
Also, check out ASAM's official [open source platform](https://github.com/asam-oss).
The structure of this list was inspired by [awesome selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted).

--------------------

- [Applications](#applications)
- [Converters](#converters)
- [Libraries](#libraries)
- [Data Structures & Models](#data-structures--models)
- [Datasets](#datasets)

--------------------

## Applications

- [CARLA](https://carla.org/) - Driving simulator based on the Unreal Engine. ([Demo](https://www.youtube.com/watch?v=7jej46ALVRE), [Source Code](https://github.com/carla-simulator/carla)) `MIT` `C++`
  - [scenario_runner](https://github.com/carla-simulator/scenario_runner) - Traffic scenario definition and execution for CARLA. `MIT` `Python`
- [esmini](https://github.com/esmini/esmini) - OpenSCENARIO player. ([Source Code](https://github.com/esmini/esmini)) `MPL-2.0` `C++`
- [OpenRoadEd](https://github.com/fhwedel-hoe/OpenRoadEd) - GUI application to create road networks in OpenDRIVE and a corresponding graphical representation in OpenSceneGraph. ([Source Code](https://github.com/fhwedel-hoe/OpenRoadEd)) `C++`
- [ODDLOT](https://www.hlrs.de/solutions-services/service-portfolio/visualization/driving-simulator/oddlot/) - GUI application for the creation of road networks and graphical representations as part of [COVISE](https://www.hlrs.de/covise/). ([Source Code](https://github.com/hlrs-vis/covise/tree/master/src/OpenCOVER/DrivingSim/oddlot)) `LGPL-2.1` `C++`
- [Blender Driving Scenario Creator](https://github.com/johschmitz/blender-driving-scenario-creator) Blender add-on for creating simple OpenDRIVE and OpenSCENARIO based driving scenarios including 3D models `GPL-3.0` `Python`

## Converters

- [r:trån](https://rtron.io) - Transformer of OpenDRIVE geometries and semantics to CityGML enabling the usage of the [3dcitydb](https://github.com/3dcitydb/3dcitydb), [FME](https://www.safe.com/fme/) and much more. ([Source Code](https://github.com/tum-gis/rtron), [Demos](https://rtron.io)) `Apache-2.0` `Kotlin`
- [OpenDRIVE2Lanelet Converter](https://commonroad.in.tum.de/opendrive_lanelet_converter) - Python converter of OpenDRIVE datasets to the Lanelet format as part of the [CommonRoad](https://commonroad.in.tum.de) project. ([Source Code](https://gitlab.lrz.de/tum-cps/opendrive2lanelet/-/tree/master)) `GPL-3.0` `Python`
- [GDAL Driver](https://github.com/DLR-TS/gdal) - OpenDRIVE driver for the library [GDAL](https://gdal.org) (translation of raster and vector geospatial data). `C++`
- [osm2opendrive](https://github.com/CWGran/osm2opendrive) - Tool for generating OpenDRIVE datasets from OpenStreetMap data. `GPL-3.0` `Python`

## Libraries

- OpenDRIVE
  - [pyeulerspiral](https://github.com/stefan-urban/pyeulerspiral) - Python implementation of euler spirals (clothoids). `MIT` `Python`
  - [C++ Object Structures](https://github.com/DLR-TS/xodr) - Data structures of OpenDRIVE 1.4 in C++. `Apache-2.0` `C++`
  - [odrSpiral](https://github.com/DLR-TS/odrSpiral) - C++ implementation of euler spirals (clothoids). `Apache-2.0` `C++`
- OpenSCENARIO
  - [openscenario.api.test](https://github.com/RA-Consulting-GmbH/openscenario.api.test) - Java library for reading and processing scenarios (C++ in progress). `Apache-2.0` `Java`
- OpenSCENARIO + OpenDRIVE
  - [scenariogeneration](https://github.com/pyoscx/scenariogeneration) - Python wrapper for parametrizing and generating linked OpenSCENARIO and OpenDRIVE datasets (formerly known as [pyodrx](https://github.com/pyoscx/pyodrx) & [pyoscx](https://github.com/pyoscx/pyoscx) project). `MPL-2.0` `Python`

## Data Structures & Models

- [OpenMaterial](https://github.com/LudwigFriedmann/OpenMaterial) - [glTF](https://github.com/KhronosGroup/glTF) extension for physical material properties in 3D models with pathtracer implementation. `MPL-2.0` `JSON`
- [Open Simulation Interface (OSI)](https://opensimulationinterface.github.io/osi-documentation/) - Generic interface based on [protobuf](https://github.com/protocolbuffers/protobuf) for the environmental perception of automated driving functions in virtual scenarios. ([Source Code](https://github.com/OpenSimulationInterface/open-simulation-interface)) `MPL-2.0`

## Datasets

- OpenDRIVE
  - [ASAM OpenDRIVE 1.6](https://www.asam.net/standards/detail/opendrive/) - Along with the official standard specification, example OpenDRIVE 1.6 datasets are distributed by ASAM.
  - [3D Mapping Solutions](https://www.3d-mapping.de/en/customer-area/) - Seven surveyed tracks in OpenDRIVE and partly in OpenCRG, including a complex intersection and the inner city of Ingolstadt (complementary to [LoD3 models](https://github.com/savenow/lod3-road-space-models)). `CC-BY-NC-SA-4.0`
  - [Atlatec](https://www.atlatec.de/getsampledata.html) - Surveyed tracks in San Francisco and in Spain along with 3D models by the company Atlatec GmbH.
  - [Brunswick](https://zenodo.org/record/4043193) - Inner ring road of Brunswick surveyed in 2012 by 3D Mapping Solutions. `CC-BY-4.0`
  - [CARLA](https://github.com/carla-simulator/opendrive-test-files) - A set of seven road networks generated with MathWorks RoadRunner.
  - [esmini](https://github.com/esmini/esmini/tree/master/resources/xodr) - Sample datasets distributed as part of esmini project.
  - [ODDLOT](https://github.com/hlrs-vis/covise/tree/master/src/OpenCOVER/DrivingSim/oddlot/samples) - Sample datasets distributed as part of ODDLOT project.
- OpenSCENARIO
  - [OSC-ALKS-scenarios](https://github.com/asam-oss/OSC-ALKS-scenarios) - Test scenarios for the approval of an "Automated Lane Keeping System" on motorways according to the [ALKS Regulation UN R157](https://undocs.org/ECE/TRANS/WP.29/2020/81). `CC-BY-SA-4.0`
