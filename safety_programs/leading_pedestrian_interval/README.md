## Leading Pedestrian Interval (LPI) 

### Description 

Leading Pedestrian Intervals (LPI) provide an advanced walk signal so that pedestrians begin to cross the street before vehicles get a green signal. This gives pedestrians more visibility within the intersection and improves motorist yielding behaviour towards pedestrians in a crosswalk. More information about LPIs can be found on [the City website](https://www.toronto.ca/services-payments/streets-parking-transportation/traffic-management/traffic-signals-street-signs/types-of-traffic-signals/leading-pedestrian-interval-phase/).

This dataset shows the intersections where LPIs are currently provided in the City of Toronto. The owner of the dataset is the Transportation Services division of the City of Toronto. 

**Format:** ESRI Shapefile (MTM 3 Degree Zone 10 NAD27)

### Relevance to the Vision Zero Challenge 

LPIs are one of the Vision Zero safety programs aimed at increasing safety at intersections for pedestrians and in particular older adults and school children.

### Data Dictionary 
| Column Name | Type | Description |
|-------------|------|-------------|
PX | Numeric | Traffic signal identifier
MAIN_STREE | Text | Main Street
MIDBLOCK_R | Text | Distance to nearest side street (device not located at an intersection)
SIDE1_STRE | Text | Side street name one
SIDE2_STRE | Text | Side street name two (if applicable)
PRIVAT_AC |  Text | Such as a driveway, laneway, entrance, etc.
ADDITIONAL | Text | Other related information
GEO_ID | Integer | End Node Identifier
NODE_ID | Integer | Intersection Node Identifier
X | Float | Easting
Y |  Float | Northing
LATITUDE |  Float | Latitude 
LONGITUDE |  Float | Longitude
ACTIVATION | Date | Date when signal was installed and put in operation (YYYY/MM/DD)
SIGNALSYST | Text | Signal system type
CONTROL_MO | Text | Control mode
PEDWALKSPE | Text | Pedestrian walking speed
AUDIBLEPED | Integer | 1 if crossing is an audible/accessible pedestrian signal (APS), 0 if it is not an APS
TRANSIT_PR | Integer | Transit priority. If the value is 0 then there is no transit nearby 
FIRE_PREEM |Integer | Fire priority - the higher the value, the closer the safety measure is to a fire station. If the value is 0, then there are no fire stations nearby.
RAIL_PREEM | Integer | Railroad priority - the higher the value, the closer the safety measure is to a railroad. if the value is 0, then there are no railroads nearby.
NUMBEROFAP | Integer | Application Number
OBJECTID | Integer | Unique system identifier
