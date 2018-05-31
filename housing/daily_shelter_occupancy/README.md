# Daily Shelter Occupancy

## Description 
The City of Toronto's Shelter, Support and Housing Administration Division maintains a list of all the active shelters serving the City of Toronto. This dataset, refreshed daily, reflects the occupancy count at each shelter at 4 a.m. each morning (established as the occupancy of the previous night).

**Format:** Comma Separated Values (CSV); JavaScript Object Notation (JSON)

The data is available on the City of Toronto's [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#711ba031-b32b-3390-ce54-22c15ac6389f).

## Relevance to the Vision Zero Challenge 
Community support services are likely used by persons that are at increased risk of being involved in a serious collision, in addition to being attractors for pedestrian trips. Pedestrians are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and are the focus of a number of existing and planned safety measures.

## Data Dictionary 
| Column Name | Type | Description |
|-------------|------|-------------|
OCCUPANCY_DATE | Text |	Count Date (DD/MM/YYYY)
ORGANIZATION_NAME	| Text | Name of the organization.
SHELTER_NAME	| Text | Name of the shelter site.
SHELTER_ADDRESS	|Text | ALocation of the shelter, address.
SHELTER_CITY	| Text | Location of the shelter, city.
SHELTER_PROVINCE	| Text  | Location of the shelter, province.
SHELTER_POSTAL_CODE	| Text | Location of the shelter, postal code.
FACILITY_NAME |Text |	Name of the facility.
PROGRAM_NAME	| Text | Name of the program within the facility.
SECTOR | Text |	Clientele of the shelter (Sector can be women, men, youth, co-ed, or family).
OCCUPANCY	| Numeric | Occupancy of the shelter at 4:00 AM the following morning.
CAPACITY | Numeric |	The total number of available beds and/or mats/cots.

Note: Supplementary information is provided on the City of Toronto's [Open Data Catalogue](https://www.toronto.ca/ext/open_data/catalog/data_set_files/Shelter_Occupancy_Metadata.xlsx)
