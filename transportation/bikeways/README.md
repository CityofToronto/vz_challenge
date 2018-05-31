# Bikeways

## Description 
The Toronto bikeways data is contained in the CP_TYPE column of the enhanced Toronto Centreline (TCL). The enhanced TCL stores linear features representing transportation corridors and boundaries, address points representing properties, doorways, sites, intersection  features and area features.

All features are attributed with feature codes, with the date they were entered into the asset and the date they were removed from the current asset to the archival asset, with identification numbers unique over time and in the city and with name, lineage and accuracy  information. The enhanced TCL also contains one-way travel information.

The Toronto bikeways data contains bicycle lanes, signed bicycle routes and pathways. It also shows suggested routes and connections in areas where routes have not yet been designated as part of the Bikeway Network. The suggested routes and connections have been identified in consultation with experienced Toronto cyclists and the Toronto Cycling Advisory Committee.

The bikeway information is appended to the enhanced Toronto Centreline file. The Toronto Centreline is a data set of linear features representing streets, walkways, rivers, railways, highways and administrative boundaries within the City of Toronto. Each line segment is described with a series of attributes including a unique identifier, name, feature code, and address ranges (where applicable).

Hhistorical bike trails data dated 2001 and 2011 are also included. 

**Format:** ESRI Shapefile (WGS84, MTM)

This dataset can be found on the [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#62a5e0cf-690e-1a8a-e8c3-81696c6f7cc9).

## Relevance to the Vision Zero Challenge
Cyclists are more vulnerable than drivers of cars, between 2005 and 2016, there were 539 cyclists killed or seriously injured in a collision with a motor vehicle in the City of Toronto. Cyclists are one of the six emphasis areas outlined in the Vision Zero Road Safety Plan. 

## Data Dictionary 

### Current Bikeways Dataset 

| Column Name | Type | Description |
|-------------|------|-------------|
GEO_ID | Integer |Unique geographic identifier for Centerlines
LFN_ID | Integer | Street Name ID
LF_NAME | Text | Full street name
ADDRESS_L| Text | Address Range on the left side of the street
ADDRESS_R| Text | Address Range on the right side of the street
OE_FLAG_L | Text | Even/Odd address numbers on left side of street
OE_FLAG_R | Text | Even/Odd address numbers on right side of street
LONUML | Integer | Lowest address number for  left side of the street segment
HINUML | Integer | Highest address number for left side of the street segment
LONUMR | Integer | Lowest address number for right side of the street segment
HINUMR | Integer | Highest address number for right side of the street segment
FNODE | Integer | Intersection id at the from node
TNODE | Intger | Intersection id at the to node
ONE_WAY_DI | Integer | Oneway direction code (0 for non-oneway, 1 follow digitized direction, -1 against digitised direction)
DIR_CODE_D | Text | Oneway code description
FCODE | Integer | Street classification
FCODE_DESC | Text | Description of the street classification
JURIS_CODE | Text | Street jurisdiction (ownership)
OBJECTID | Integer | Unique system identifier
CP_TYPE | Text | Bikeway Type Description

## Linear Feature Description 
Highway is designated for fast, long distance travel with restricted access to sustain high speeds. 

Highway Transfer Ramp provides for transfer between road and highway and also between highway and highway. 

Arterial Road is usually under regional jurisdiction and is fed by collector roads and in some cases is connected to other arterial roads or collector roads via Road Ramp. 

Collector Roads is designated mainly for travel to and from arterial roads with some driveway  access. In Metro they are usually under local jurisdiction.

Lane is designated mainly for City of Toronto laneways and are usually under local jurisdiction.

Local Road is designated to service driveway access and usually connects to collector roads or other local roads.

Access Road is dedicated to provide access to or within properties such as townhouse complexes, airports etc.

Pending Road is suggested to identify roads with a planned feature code that awaits Council Approval. This is not requested until the road is assumed and may be delayed for 6 years or more.

Road Ramps (major arterial,minor arterial, collector, other) provides for transfer between two roads.

Busway is a road dedicated for buses only.

Major Railway is designated for the fast, long distance, inter-provincial movement of cargo or passenger trains. 

Minor Railway is designated for local public transportation and includes above ground rapid transit corridors and subway lines.

River is a major waterway. 

Creek/Tributary is a minor waterway.

Trail is a pedestrian way designated for recreational purposes and can include foot-powered vehicles such as bikes or roller-blades etc. 

Walkway is a designated path primarily for walking.

Hydro Line is an electricity transportation corridor (high voltage).

Major Shoreline is a boundary of a large body of water. E.g. Lake Ontario shoreline. 

Minor Shoreline is a boundary of a small body or water such as a pond or reservoir.

For more information on road classification, see the City of Toronto page on the [road classification system](https://www.toronto.ca/services-payments/streets-parking-transportation/traffic-management/road-classification-system/).

## Street Feature Codes 
Every linear feature has feature code (FCODE) defined as follow:

| FCODE | Description |
|-------------|-------------|
201100 |Highway
201101 | Highway Ramp
201200 | Major Arterial Road
201201	| Major Arterial Road Ramp
201300	| Minor Arterial Road
201301	| Minor Arterial Road Ramp
201400	| Collector Road
201401	| Collector Road Ramp
201500	| Local Road
201600	| Other Road
201601	| Other Ramp
201700	| Laneways
201800	| Pending
201803  | Access Road
201801  | Busway
202001	| Major Railway
202002	| Minor Railway
202003	| Railway under construction/proposed
203001	| River
203002	| Creek/Tributary
204001	| Trail
204002	| Walkway
205001	| Hydro Line
206001	| Major Shoreline
206002	| Minor Shoreline (Land locked)


## Street Type Abbreviations
| Type Part of Linear Feature Name | Abbreviation |
|-------------|-------------|
Avenue | Ave
Bridge	| Bdge
Boulevard	| Blvd
Circle | Crcl
Court | Crt
Circuit | Crct
Cresent | Cres
Close | Cs
Drive | Dr
Expressway | Xwy
Garden | Gdn
Gardens | Gdns
Gate | Gt
Green | Grn
Grove | Grv
Heights | Hts
Highway | Hwy
Hill | Hill
Lane | Lane
Lawn | Lwn
Line | Line
Mews | Mews
Park | Pk
Parkway | Pkwy
Path | Path
Pathway | Ptwy
Place | Pl
Promenade | Prom
Ramp | Ramp
Road | Rd
Roadway | Rdwy
Square | Sq
Street | St
Terrace | Ter
Trail | Trl
View | View
Walk | Walk
Way | Way
Woods | Wds

### Historical Bike Trails Dataset 

| Column Name | Type | Description |
|-------------|------|-------------|
LF_NAME	| Text | Long form name
JURIS_CODE | Text | Jurisdiction code 
STR_NAME	| Text | Street name
ROOT_ID	| Text | Root ID
SEGMENT	| Text | Order of the segment in the route 
SEG_TYPE | Text | Segment Type (i.e. bike lane, off road, signed route)
STATUS | Text | Indicates whther the bike trail is existing or a proposed bike trail
STATUS_SEG | Text | The STATUS column concatenated with the SEG_TYPE column
INSTALLATI | Integer | Year of installation
RouteNum | Integer | Route ID
District | Text | District name
Ward | Integer | Ward number


