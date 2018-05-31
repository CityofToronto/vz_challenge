# Toronto Community Housing

## Description
The City of Toronto's Economic Development & Culture Division owns this dataset, which is a list of all Toronto Community Housing (TCH) developments with more than five units. The data is current as of May 2015.

**Format:** ESRI shapefiles (MTM 3 Degree Zone 10 NAD27, WGS84)

The file is available on the City of Toronto's [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#3cbd0ba7-4bb2-923d-89d2-aff78797fe55).

## Relevance to the Vision Zero Challenge
TCH developments may be linked to segments of the population that are at increased risk of being involved in a serious collision.

## Data Dictionary

|Column Name|Type|Description
|-----|-----|-----|
OBJECTID|Integer|Unique identifier for the dataset.
BLD_ID|Float|A unique identifier of the building.
DEV_ID|Float|A unique identifier of the site/development.
DEV_NAME|Text|The name of the TCH development.
NGHDNHM|Integer|TCH District that the development is located in.
POLICEDIVI|Float|Police division that the development is located in.
BLDG_POSTC|Text|Postal code.
TOTAL_RESU|Float|Total number of units.
MRKT_UNIT|Float|Total number of market priced units.
RGI_UNIT|Float|Total number of rent-geared-to-income units.
YEAR_BUILT|Float|Year the development was built.
BUILDING|Text|Category of building.
BUILDFORM|Text|Specific details about the building.
FLR_ABV_GR|Float|Floors the building has.
BLD_DESC|Text|Building description including the number of floors and building details.
X|Float|X coordinate, MTM3 Zone 10.
Y|Float|Y coordinate, MTM3 Zone 10.
LONGITUDE|Float|Longitude, WGS84.
LATITUDE|Float|Latitude, WGS84.
