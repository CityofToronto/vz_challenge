# Crossing Guard Location

## Description
The Traffic Safety Unit of the City of Toronto provides [this dataset](crossing_guards.zip) `crossing_guards.zip`, which lists every intersection where there is a crossing guard to aid children and people crossing the road near school grounds. The dataset is current to 2017.

**Format:** ESRI Shapefile

## Relevance to the Vision Zero Challenge
Crossing guard locations help identify intersections of the city that already have safety measures in place to prevent vehicular incidents with children and people. School children are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and are the focus of a number of existing and planned safety measures.

## Data Dictionary
| Column Name | Type | Description |
|-------------|------|-------------|
wkt_geom  | Float | Coordinates in XY format
Location | Text | Unique Identifier
Main_St|Text|The primary road at the intersection
Cross_St|Text|The secondary road at the intersection
Toronto_Di|Text|The TCDSB school this crossing guard serves
Toronto_1|Text|The TDSB school this crossing guard serves
Remove|Text|Date that crossing guards were removed
Type|Text|Type of intersection. PXO refers to pedestrian crossing
District|Text|The district (Etobicoke, Scarborough, North York, Toronto and East York) the crossing guard is located in
