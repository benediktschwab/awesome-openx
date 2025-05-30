# Awesome OpenX [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

A curated list of awesome applications, libraries and datasets concerning the development and testing of automated driving functions with a focus on [ASAM OpenX Standards](https://www.asam.net/standards/) (e.g. [OpenDRIVE](https://www.asam.net/standards/detail/opendrive/), [OpenSCENARIO](https://www.asam.net/standards/detail/openscenario/), [OpenLABEL](https://www.asam.net/standards/detail/openlabel/), ...).

This is a list of [free](https://en.wikipedia.org/wiki/Free_software) software and datasets, whereas non-free software will be listed on the [non-free](non-free.md) page.
Also, check out ASAM's official [open source platform](https://github.com/asam-oss).
The structure of this list was inspired by [awesome selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted).

--------------------

- [Applications](#applications)
- [Converters](#converters)
- [Libraries](#libraries)
- [Data Structures & Models](#data-structures--models)
- [Datasets](#datasets)
- [Miscellaneous](#miscellaneous)

--------------------

## Applications

- [CARLA](https://carla.org/) - Driving simulator based on the Unreal Engine. ([Demo](https://www.youtube.com/watch?v=7jej46ALVRE), [Source Code](https://github.com/carla-simulator/carla)) `MIT` `C++`
  - [scenario_runner](https://github.com/carla-simulator/scenario_runner) - Traffic scenario definition and execution for CARLA. `MIT` `Python`
- [esmini](https://github.com/esmini/esmini) - OpenSCENARIO player. ([Source Code](https://github.com/esmini/esmini)) `MPL-2.0` `C++`
- [OpenRoadEd](https://github.com/fhwedel-hoe/OpenRoadEd) - GUI application to create road networks in OpenDRIVE and a corresponding graphical representation in OpenSceneGraph. ([Source Code](https://github.com/fhwedel-hoe/OpenRoadEd)) `C++`
- [ODDLOT](https://www.hlrs.de/solutions/types-of-computing/visualization/oddlot) - GUI application for the creation of road networks and graphical representations as part of [COVISE](https://www.hlrs.de/covise/). ([Source Code](https://github.com/hlrs-vis/covise/tree/master/src/oddlot)) `LGPL-2.1` `C++`
- [Blender Driving Scenario Creator](https://github.com/johschmitz/blender-driving-scenario-creator) - Blender add-on for creating simple OpenDRIVE and OpenSCENARIO-based driving scenarios, including 3D models. `GPL-3.0` `Python`
- [Unreal Engine OpenDRIVE plugin](https://github.com/brifsttar/OpenDRIVE) - Plugin for creating and manipulating OpenDRIVE road networks based [esmini](https://github.com/esmini/esmini)'s [RoadManager](https://github.com/esmini/esmini/tree/master/EnvironmentSimulator/Modules/RoadManager). `MPL-2.0` `C++`
- [LaneMaker](https://github.com/guotata1996/lanemaker) - Qt5 GUI application for creation of 3D road networks which can be exported to OpenDRIVE `Apache-2.0` `C++`

## Converters

- [r:trån](https://rtron.io) - Transformer of OpenDRIVE geometries and semantics to CityGML enabling the usage of the [3dcitydb](https://github.com/3dcitydb/3dcitydb), [FME](https://www.safe.com/fme/) and much more. ([Source Code](https://github.com/tum-gis/rtron), [Demos](https://rtron.io)) `Apache-2.0` `Kotlin`
- [OpenDRIVE2Lanelet Converter](https://commonroad.in.tum.de/opendrive_lanelet_converter) - Python converter of OpenDRIVE datasets to the Lanelet format as part of the [CommonRoad](https://commonroad.in.tum.de) project. ([Source Code](https://gitlab.lrz.de/tum-cps/opendrive2lanelet/-/tree/master)) `GPL-3.0` `Python`
- [OpenDRIVE to NetworkX and GeoPandas Converter](https://github.com/larsklitzke/xodr2nxgpd/) - Converter of OpenDRIVE geometries to [`geopandas.GeoDataFrame`](https://geopandas.org/en/stable/docs/reference/api/geopandas.GeoDataFrame.html) and network intersections to [NetworkX](https://networkx.org/), using OpenDRIVE2Lanelet Converter. `MIT` `Python`
- [GDAL Driver](https://dlr-ts.github.io/gdal-opendrive-how-to/) - OpenDRIVE driver for the library [GDAL](https://gdal.org) (translation of raster and vector geospatial data). `C++`
- [osm2opendrive](https://github.com/CWGran/osm2opendrive) - Tool for generating OpenDRIVE datasets from OpenStreetMap data. `GPL-3.0` `Python`
- [osm2xodr](https://github.com/JHMeusener/osm2xodr) - Tool for generating OpenDRIVE datasets from OpenStreetMap data. `GPL-3.0` `Python`

## Libraries

- OpenDRIVE
  - [pyeulerspiral](https://github.com/stefan-urban/pyeulerspiral) - Python implementation of euler spirals (clothoids). `MIT` `Python`
  - [C++ Object Structures](https://github.com/DLR-TS/xodr) - Data structures of OpenDRIVE 1.4 in C++. `Apache-2.0` `C++`
  - [odrSpiral](https://github.com/DLR-TS/odrSpiral) - C++ implementation of euler spirals (clothoids). `Apache-2.0` `C++`
  - [libOpenDRIVE](https://github.com/grepthat/libOpenDRIVE) - Lightweight, fast C++ library providing OpenDRIVE file parsing and 3D model generation as well as a [web-based viewer](https://odrviewer.io/). `Apache-2.0` `C++`
- OpenSCENARIO
  - [openscenario.api.test](https://github.com/RA-Consulting-GmbH/openscenario.api.test) - Java library for reading and processing scenarios. `Apache-2.0` `C++`
- OpenSCENARIO + OpenDRIVE
  - [scenariogeneration](https://github.com/pyoscx/scenariogeneration) - Python wrapper for parametrizing and generating linked OpenSCENARIO and OpenDRIVE datasets (formerly known as [pyodrx](https://github.com/pyoscx/pyodrx) & [pyoscx](https://github.com/pyoscx/pyoscx) project). `MPL-2.0` `Python`
- OpenLABEL
  - [Video Content Description (VCD)](https://github.com/Vicomtech/video-content-description-VCD) - API for creating and editing JSON data compliant with OpenLabel 1.0. `MIT` `Python` `TypeScript` `C++`
- Open Simulation Interface (OSI)
  - [OpenSimulationInterface.CSharp](https://github.com/thempen/open-simulation-interface-csharp) - [NuGet](https://www.nuget.org/packages/OpenSimulationInterface.CSharp) package for using OSI in C#/.NET. `MPL-2.0` `C#` `Protobuf`

## Data Structures & Models

- [OpenMaterial](https://github.com/LudwigFriedmann/OpenMaterial) - [glTF](https://github.com/KhronosGroup/glTF) extension for physical material properties in 3D models with pathtracer implementation. `MPL-2.0` `JSON`
- [Open Simulation Interface (OSI)](https://opensimulationinterface.github.io/osi-documentation/) - Generic interface based on [protobuf](https://github.com/protocolbuffers/protobuf) for the environmental perception of automated driving functions in virtual scenarios. ([Source Code](https://github.com/OpenSimulationInterface/open-simulation-interface)) `MPL-2.0`
- [OpenMSL](https://github.com/openmsl) - The Open Source Model & Simulation Library is a central hub demonstrating the interaction between models, standards and tools. `MPL-2.0`

## Datasets

- OpenDRIVE
  - [ASAM OpenDRIVE 1.7.0](https://www.asam.net/standards/detail/opendrive/) - Along with the official standard specification, example OpenDRIVE 1.7.0 datasets are distributed by ASAM.
  - [3D Mapping Solutions](https://www.3d-mapping.de/en/customer-area/) - Seven surveyed tracks in OpenDRIVE and partly in OpenCRG, including a complex intersection and the inner city of Ingolstadt (complementary to [LoD3 models](https://github.com/savenow/lod3-road-space-models)). `CC-BY-NC-SA-4.0`
  - [German Autobahn A9](https://mobilithek.info/offers/573178449617657856) - Two sections of the German Autobahn A9 with a total length of 52km ([Mirror](https://github.com/tum-gis/opendrive-testfeld-a9)).
  - [TUMDOT-MUC](https://www.mos.ed.tum.de/en/vt/research/data-sets/tumdot-muc/) - Vehicle trajectories observed from aerial drones with accompanied OpenDRIVE map. ([Article](https://doi.org/10.1007/s42421-024-00101-5)) `CC-BY-NC-4.0`
  - [Brunswick "Schwarzer Berg"](https://doi.org/10.5281/zenodo.15395839) - "Schwarzer Berg" region in Brunswick surveyed in 2024 by 3D Mapping Solutions. `CC-BY-4.0`
  - [Brunswick ring road](https://doi.org/10.5281/zenodo.4043192) - Inner ring road of Brunswick surveyed in 2012 by 3D Mapping Solutions. `CC-BY-4.0`
  - [Brunswick ring road to airport](https://doi.org/10.5281/zenodo.7071845) - ViVre research track in Brunswick surveyed in 2021 by 3D Mapping Solutions. `CC-BY-4.0`
  - [Wolfsburg](https://doi.org/10.5281/zenodo.7072630) - 5G Living Lab research track in Wolfsburg surveyed in 2022 by Atlatec. `CC-BY-4.0`
  - [CARLA](https://github.com/carla-simulator/opendrive-test-files) - A set of seven road networks generated with MathWorks RoadRunner.
  - [esmini](https://github.com/esmini/esmini/tree/master/resources/xodr) - Sample datasets distributed as part of esmini project.
  - [ODDLOT](https://github.com/hlrs-vis/covise/tree/master/src/OpenCOVER/DrivingSim/oddlot/samples) - Sample datasets distributed as part of ODDLOT project.
- OpenSCENARIO
  - [OSC-ALKS-scenarios](https://github.com/asam-oss/OSC-ALKS-scenarios) - Test scenarios for the approval of an "Automated Lane Keeping System" on motorways according to the [ALKS Regulation UN R157](https://undocs.org/ECE/TRANS/WP.29/2020/81). `MPL-2.0`
  - [OSC-NCAP-scenarios](https://github.com/vectorgrp/OSC-NCAP-scenarios) - Test scenarios for the verification of "Automated Emergency Braking (AEB)" and "Lane Support Systems (LSS)" according to [Euro NCAP](https://www.euroncap.com/) protocols. `MPL-2.0`

## Miscellaneous

- Nicco Hagedorn's [YouTube channel](https://www.youtube.com/watch?v=2pX2dJL0Jnc&list=PLUv2R7fQV7GVLgrCzrtyAnLUzdtjYx9N9&index=6) - Concise explanations of the OpenDRIVE concepts along with practical examples compiled in a video series.
