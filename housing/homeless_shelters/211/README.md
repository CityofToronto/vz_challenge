# Homeless Shelters (211 Data)

## Description
211 Toronto owns [this dataset](housing_shelters_211.csv) `housing_shelters_211.csv`, which is a list of additional homeless shelters in Toronto that are not found in the [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#f6f92858-b907-7ac1-808b-0778923e72ca) dataset, but are found on 211 Toronto. The data includes the locations of both not-for-profit shelters and city-run shelters.

**Format:** Comma-Separated Values (CSV); also available as [GeoJSON](housing_shelters_211.geojson) and [ESRI Shapefile](housing_shelters_211.zip)

## Relevance to the Vision Zero Challenge
Homeless shelter are used by people who are likely to walk to the centres and are at-risk of collisions with vehicles. Pedestrians are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and as such are the focus of a number of existing and planned safety measures.

## Data Dictionary
Column|Type|Description
|-----|-----|-----|
ID|Text|A unique identifier.
NAME|Text|The name of the shelter.
ADDRESS|Text|The street address of the shelter
LATITUDE|Float|Latitude
LONGITUDE|Float|Longitude
POSTAL|Text|Postal code

## Limitations
This data is not exhaustive of all homeless shelters in Toronto. The data contains unique entries compared to the list of shelters found on the [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#f6f92858-b907-7ac1-808b-0778923e72ca) and is intended to be used as a supplement to that dataset. There are no duplicates between the two datasets. This data relies on a shelter to list itself on 211 Toronto, and even together the two datasets may not include every homeless shelter in Toronto.
