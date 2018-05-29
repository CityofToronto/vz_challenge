## Leading Pedestrian Interval (LPI) 

### Description 

The Leading Pedestrian Interval (LPI) program provides an advanced walk signal so that pedestrians begin to cross the street before vehicles get a green signal. The purpose of LPI is to provide pedestrians an advantage over turning vehicles at intersections where it is determined that pedestrians, wishing to enter the crosswalk, were being hindered by aggressive right turns. The LPI is used to improve motorist yielding behaviour toward pedestrians in a crosswalk. The LPI is particularly helpful for older pedestrians, as they may take longer to occupy the crosswalk following the start of a “walk” indication, making them less obvious to turning motorists.

More information about LPIs can be found on [the City website](https://www.toronto.ca/services-payments/streets-parking-transportation/traffic-management/traffic-signals-street-signs/types-of-traffic-signals/leading-pedestrian-interval-phase/).

This dataset details the locations of the LPIs in the City of Toronto. The data is available in Shapefile format with the MTM 3 Degree Zone 10 NAD27 projection, and is uploaded in this GitHub directory. The owner of the dataset is the Transportation Services division of the City of Toronto. 

### Relevance to the Vision Zero Challenge 

LPIs were created to help pedestrians, especially older adults, to cross an intersection safely while limiting potential interactions with vehicles. 

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