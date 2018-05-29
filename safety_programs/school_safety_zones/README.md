# School Safety Zones


## Description

This data contains the information on the schools located in existing School Safety Zones in the City of Toronto. Information includes address and geographic coordinates, as well as the school population. The data is owned by the City of Toronto's Transportation Services Division, and is available in the form of a shapefile with the MTM 3 Degree Zone 10 NAD27 projection.

## Relevance to the Vision Zero Challenge

School Children are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and as such are the focus of a number of existing and planned safety measures. School Safety Zones include a variety of measures such as lower speed limits, improved street lighting, leading pedestrian intervals, mid-block crossings, increased enforcement, improved pavement makings, flashing signage and/or public awareness campaigns, among other possible improvements.

## Data Dictionary

|Column|Type|Description|
|-----|-----|-----|
GEO_ID|Integer|Identifier of the centreline road segment that the school zone is located on.
SCHOOL_NAM|Text|Name of the school.
BOARD_NAME|Text|Name of the school board.
ADDRESS_NU|Integer|Numeric address of the school.
LINEAR_NAM|Text|Street where the school is located.
POSTAL_COD|Text|Postal code of the school.
WARD|Integer|Ward in which the school is located.
DISCTRICT|Text|District of Toronto in which the school is located in.
LATITUDE|Float|Latitude of the school.
LONGITUDE|Float|Longitude of the school.
SCHOOL_POP|Integer|Number of students attending the school.
F__OF_POP|Float|Percentage of students living within walking distance (1.6km) of the school.
