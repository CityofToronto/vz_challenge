# TTC Stops

## Description
The Toronto Transit Commission (TTC) maintains a dataset, [`TTC_stops.zip`](shp/TTC_stops.zip), that contains the locations of all stops being used by bus and streetcar routes in the TTC network, including temporary and inactive stops. Each stop has a stop ID that is can be linked with the [TTC Ridership dataset](../ttc_ridership), the TTC website, transit navigation services such as Google Maps, and the General Transit Feed Specification (GTFS). The dataset was last updated in 2018.

**Format:** ESRI Shapefile (WGS84)

## Relevance to the Vision Zero Challenge
Transit stops are locations at which pedestrians enter and leave the transit network. Pedestrians are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and is the focus of a number of existing and planned safety measures.

## Data Dictionary
|Column Name|Type|Description|
|:-----|:-----|:-----|
Feature Nu|Integer|Stop ID for each stop.
On Street|Text|Street, building, subway station, or loop that the stop is on
At Street|Text|Intersecting street, building, subway station, or loop that the stop is on.
Direction|Text|Direction of traffic that the stop is on.
Location|Text|Whether the stop is located the near-side or far-side of an intersection. This field can also specify whether the stop is at a subway station or mid-block.
Seq|Integer|A differentiator between stops if there are multiple stops at the same location, or if there is a temporary stop replacing a permanent stop.
Bay|Text|Indicator if the stop has a bus bay/pullout. This field is blank if there is no bus bay.
Island|Text|Indicator if the stop is on a traffic island (such as some streetcar stops). This field is blank if there is no island.
Shelter|Text|Indicator if the stop has a shelter. This field is blank if there is no shelter. If there are any conflicts with the [Transit Shelters dataset](../transit_shelters), the Transit Shelters dataset takes precedence.
GF_COORD_L|Float|Latitude, WGS84.
GF_COORD_1|Float|Longitude, WGS84.
