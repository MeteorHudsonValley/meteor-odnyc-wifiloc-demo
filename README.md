# meteor-odnyc-wifiloc-demo
Simple demo to showcase usage of the nitya:odnyc-wifiloc package.

### Attribution
See the [nitya:odnyc-wifiloc] package repo (https://github.com/nitya/meteor-odnyc-wifiloc) for attribution related to dataset and package

### Demo
A version of the demo app is running at [odnyc-wifilocs.meteor.com](http://odnyc-wifilocs.meteor.com)

The demo uses the [Leaflet](http://leafletjs.com/) library to dynamically show markers for all the WiFi hotspots listed in the city dataset. Markers are bound to pop-ups that show additional details from the dataset (related to that hotspot).

*TODO*
Currently the demo uses a Session variable to store the query that is used to filter/retrieve a relevant subset of WiFi location records - e.g., currently the query looks for all hotspots of Type=Library.

The code needs to be updated to instead allow query criteria to be dynamically shown/selected from the map itself. To support this, there is a TODO on the package that exports Metadata for the WifiLocs dataset which could provide enumerated constants or other information useful in querying.