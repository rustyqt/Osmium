Osmium
======

**Osmium** is a fork of **OsmAnd~** — the fully-featured, F-Droid build of [OsmAnd](https://github.com/osmandapp/OsmAnd), the offline maps & navigation app powered by OpenStreetMap data.

Osmium is built from the OsmAnd source and stays close to it. It is rebranded (own name, launcher icon and application id `net.osmand.osmium`, so it installs **alongside** a stock OsmAnd / OsmAnd~) and adds a small set of extra features.

What Osmium adds on top of OsmAnd~
----------------------------------

* **Rebranding** — the name "Osmium", a distinct launcher icon, and the application id `net.osmand.osmium` so it coexists with OsmAnd on the same device.
* **Dashed track lines** — in the saved-track **Appearance** editor you can draw a track as a **dashed line**. The setting is stored per track (in the track database and in the GPX `<extensions>`). *A second, alternating dash colour is the next planned step.*

Everything else is OsmAnd: offline vector maps, turn-by-turn navigation (car / bicycle / pedestrian), search, GPX trip recording, POIs, contour lines & hill-shading, and more.

Building
--------

Osmium builds exactly like OsmAnd. The native rendering core is downloaded as a prebuilt artifact, so no C++ / Skia / Qt build is required:

```
./gradlew :OsmAnd:assembleAndroidFullOpenglArm64Debug
```

Requirements: JDK 17, Android SDK (platform 35, build-tools 35.0.0). The `OsmAnd-resources` repository must be checked out as a sibling `../resources` directory. See the OsmAnd build documentation: https://osmand.net/docs/technical/build-osmand/

Credits & licence
-----------------

Osmium is a derivative work of **OsmAnd** and is distributed under the same licence (see `LICENSE`). Map data © OpenStreetMap contributors. All credit for the underlying application belongs to the OsmAnd team — please support the upstream project at https://osmand.net.

---

OsmAnd features (inherited)
---------------------------

#### Navigation
 * Works online (fast) or offline (no roaming charges abroad)
 * Turn-by-turn voice guidance (recorded and synthesized voices)
 * Optional lane guidance, street-name display, and estimated time of arrival
 * Intermediate points and automatic re-routing
 * Search by address, by type (restaurant, hotel, fuel, …) or by coordinates

#### Map viewing
 * Position & orientation on the map, optional compass / motion alignment
 * Favourites and surrounding POIs
 * Online tile maps and satellite overlays with adjustable transparency
 * GPX track overlays
 * Place names in English, local, or phonetic spelling

#### OpenStreetMap & Wikipedia data
 * Global, per-country/region map downloads — compact offline vector maps
 * Frequently updated; optional Wikipedia POIs

#### Outdoor
 * Foot, hiking and bike paths; dedicated bicycle / pedestrian routing
 * Trip recording to GPX, speed/altitude display, contour lines & hill-shading

#### Contribute to OpenStreetMap
 * Report map bugs, add POIs, and upload GPX tracks directly from the app

Worldwide map coverage from OpenStreetMap data.
