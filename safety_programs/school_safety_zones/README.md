# School Safety Zones


## Description

This data lists the location of existing School Safety Zones in the City of Toronto. School Safety Zones are deployed at prioritized schools and include a variety of measures such as school zone pavement markings, "Watch Your Speed" driver feedback signs, zebar markings at crosswalks improved street lighting, reduced speed limits, leading pedestrian intervals, mid-block crossings, increased enforcement, improved pavement makings, flashing signage and/or public awareness campaigns, among other potential improvements.

This dataset includes address and geographic coordinates, school population and an estimate of the percentage of students living within walking distance of the school. The data is maintained by the City of Toronto's Transportation Services Division.

**Format:** ESRI Shapefile (MTM 3 Degree Zone 10 NAD27)

## Relevance to the Vision Zero Challenge

School Safety Zones are an important safety program targetted at improving the safety of school children. School children are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan.

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
