# Turn Restrictions

## Description 

This dataset details streets in Toronto where one may turn, the turn direction, and any restrictions (such as the types of vehicles
allowed on the street or the types of turns allowed). This dataset also shows the locations of ramps, channelized right turns, and dedicated turn lanes. There are two shapefiles (`Centreline_flow_wgs84` and `Turn_Restrictions_wgs84`) and two `dbf` tables (`time_limitaition` and `time_limitaition_detail` (typos in original)) included in this dataset. `dbf` files can be opened in Excel, or joined to the shapefiles using GIS software.

This dataset is available through the [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#6b9a0b86-ae27-af95-13fc-8e434b2b7bc6) and is current to 2017.

## Relevance to the Vision Zero Challenge 

Turn restrictions are a tool by transportation engineers to improve the speed and reliability of transit, improve intersection safety by removing dangerous maneuvers/conflicts and reduce the congestion impacts of turns. Turn restrictions improve safety by reducing pedestrian collisions, reducing collisions involving turning vehicles, and reduce the possibility of vehicles blocking the intersection. 

Ramps and channelized turns increase the speed of turning vehicles which may increase pedestrian danger.  

## Data Dictionary

### Notes:
1. Centreline should be used as background
2. Use Geographic ID (`GEO_ID`) to link centreline with turns dataset.
3. Link `Turn_Restrictions` to limitation tables (`time_limitaition` and `time_limitaition_detail`) using the `Limitation` column.
4. For routing we recommend using the centreline_id, Turn restrictions and limitation tables, and the flow dataset.

### Turn_Restrictions
| Field | Type | Field Description |
|-------------|------|-------------|				
FID | Integer |  Uniquely identifies each row
TURN_ID  | Integer | Uniquely identifies each turn 
INTERSECTI | Integer | Unique identifier for intersections		
CONNECTIVI | Integer | First connectivity identifier 				
CENTRELINE | Integer | First centreline identifier (known as GEO_ID in centreline table)				
CONNECTI_1 | Intger | Second connectivity identifier	
CENTRELI_1 | Integer | Second centreline identifier 				
TURN_ANGLE | Integer | Angle of turn 			
TURN_DIR_C | Text | Turn direction code (i.e. 'RIGHT', 'UTURN', etc.) 		
TRAVEL_MOD  | Integer | Travel mode code				
TRAVEL_M_1  | Text | Travel mode description			
TURN_PERMI | Integer | Turn permission code 			
TURN_PER_1 | Text | Turn permission description		
TURN_IMPED | Integer | Turn impedance
LIMITATION | Integer | Limitation ID
LIMITATI_1 | Integer | Limitation type
LIMITATI_2 | Text | Limitation type description 
LIMITATI_3 | Integer | Limitation permission
LIMITATI_4 | Text | Limitation permission description
LIMITATI_5 | Integer | Limitation impedance	
OBJECTID | Integer | Internal shapefile column

### Centreline_flow
| Field | Type | Field Description |
|-------------|------|-------------|										
FID | Integer | Internal shapefile column									
SHAPE | Integer | Internal shapefile column
CONNECTIVI | Integer | Flow ID (Connectivity identifier)									
INTERSECTI | Integer | Unique id of the intersection									
CENTRELINE | Integer | Unique id of the centreline segment flowing into the intersection						AZIMUTH | Integer | Azimuth of the line segment at the intersection							
ARC_END	| Text| The FROM or TO of the centreline segment at the intersection 							
OBJECTID  | Integer | Unique system identifier						
CROSSING_L | Integer | Elevation level or crossing level. 0 is lowest (0 Base, 1 first level, 2 second level, etc)

The centreline flow layer contains information about how traffic can move into each intersection from the City of Toronto centreline. The file is not a full centreline file, it only contains information at intersections. A given centreline from the TCL may have two lines represented in the centreline flow layer for the intersection at either end of the line.

### time_limitation Table
| Field | Type | Field Description |
|-------------|------|-------------|
OID | Integer | Internal shapefile column
LIMITATION 	| Integer | Limitation ID
LIMITATI_1  | Integer | Limitation type/class
LIMITATI_2 | Text | Limitation type description 

### time_limitation_detail Table
| Field | Type | Field Description |
|-------------|------|-------------|
OID | Integer | Internal shapefile column
DETAIL_ID | Integer | Detail ID 
LIMITATION | Integer | Limitation ID
TYPE_OF_DA | Text | Type of Day
DAY_FROM | Integer | Day of the week that the limitation on the road starts
DAY_TO | Integer | Day of the week that the limitation on the road ends
TIME_START | Integer | Time of the day (24 HR) that the limitation starts
TIME_END | Integer |  Time of the day (24 HR) that the limitation ends
					
### Limitations

This dataset is not current, and may not reflect legal restrictions currently in place on the City's streets. Always obey street signage over data provided here.

The Toronto CentreLine version is not current, and this dataset may not line up with other datasets using the TCL.
