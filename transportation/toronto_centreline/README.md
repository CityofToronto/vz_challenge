# Toronto Centreline (TCL)

## Description
The Toronto Centreline (TCL) is a geographic dataset of linear features representing streets, walkways, rivers, railways, highways and administrative boundaries within the City of Toronto. Each line segment is described with a series of attributes including a unique identifier, name, feature code, and address ranges (where applicable). For the `centreline_lengths` files, there is an additional field for segment length.

**Format:** ESRI Shapefile (WGS84; NAD2 UTM Zone 17N); Comma Separated Values (CSV); GeoJSON

The data is available on the City of Toronto's [Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#e4ec3384-056f-aa59-70f7-9ad7706f31a3).

## Relevance to the Vision Zero Challenge
The Toronto Centreline (TCL) provides a base layer on which transportation infrastructure is built, and which many transportation datasets are referenced against.

## Data Dictionary
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
TNODE | Intger | To intersection id
FCODE | Integer | Street classification
FCODE_DESC | Text | Description of the street classification
JURIS_CODE | Text | Street jurisdiction (ownership)
OBJECTID | Integer | Unique system identifier
LENGTH_M | Numeric | Length of the segment, in metres. Only in the `centreline_lengths` files

Additional metadata related to specific fields in the dataset are available in documentation within the shapefile package.
