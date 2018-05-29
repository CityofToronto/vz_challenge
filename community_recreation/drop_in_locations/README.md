# Drop-In Locations (Toronto Drop-In Network Members - TDIN)

## Description 
The Toronto Drop-In Network (TDIN) is an active coalition of drop-in centres working with people who are homeless, marginally housed or socially isolated in Toronto. Their network includes drop-ins of all sizes and diverse philosophies serving men, women, youth, seniors and families. This dataset contains the locations of drop-in centres within the City of Toronto that are members of TDIN.

The dataset is a City-wide GIS point file and can be linked to the City's Street Centreline file.

The data is current as of February 2012, and is owned by the City of Toronto's Shelter Support & Housing Administration Division, and is provided as ESRI shapefiles (MTM 3 Degree Zone 10 NAD27 and WGS84 Latitude/Longitude projections). The data is availiable through the City of Toronto's [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#0365988c-3ead-45f4-d25d-6dbdeb7a8720).

## Relevance to the Vision Zero Challenge 
The locations of drop-in centres in Toronto could be linked to populations at higher risk of involvement in a serious collision. They may also attract significant amounts of pedestrian traffic.

## Data Dictionary 
| Column Name | Type | Description |
|-------------|------|-------------|
FID	| Numeric | Unique Feature Identifier	
SHAPE	| Text | Feature type (e.g. point)
ADDRESS_PO | Numeric | Unique geographical Address Identifier
ADDRESS	| Text | Full municipal address	
POSTAL_COD	| Text | Postal code	
MUNICIPALI	| Text |Former city municipality	
CITY | Text |Toronto	
CENTRELINE |	Numeric |The unique geographic identifier of the street segment the address is on
OBJECTID |Numeric|	Object identifier 	
NAME	| Text | Name of drop-in location 
ORGANIZA_1 | Text | Name of Organization running the Drop-In
Facility | Text | Name of place hosting the Drop-In
