# Red Light Cameras

## Description
This dataset provides a list of all locations at which Red Light Cameras (RLCs) are currently installed. RLCs are used to capture an image of a vehicle that has entered an intersection during the red phase of a traffic signal. They are used to help enforce compliance with traffic laws, and to reduce the potential for collisions at priority locations.  This dataset is owned and maintained by the City of Toronto's Transportation Services Division, and is current as of January 2018. 

## Relevance to the Vision Zero Challenge
Red Light Camera locations can be used to determine where safety measures have been targeted to-date, and to potentially evaluate their effectiveness in reducing speeding, collisions, and other adverse events.

## Data Dictionary

|Column Name|Type|Description|
|-----|-----|-----|
OBJECTID|Integer|A unique GIS identifier of each location with a red light camera.
PX|Integer|Signalized intersection identifier linking back to the City's Traffic Signals dataset
Main|Text|Main street of the intersection.
Side_1_Rou|Text|Cross street of the intersection.
Side_2_Rou|Text|Secondary crossing street at the intersection, if applicable.
Private_Ac|Text|Additional details of the type of private access.
Additional|Text|Additional notes on the location of the intersection.
Geo_ID|Integer|Road segment from the Centreline file with which the camera is associated.
Node_GeoID|Integer|Intersection from the Centerline Intersections file at which the camera is located.
X|Float|X coordinate
Y|Float|Y coordinate
Latitude|Float|Latitude
Longitude|Float|Longitude
