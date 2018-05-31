# Places of Worship 

## Description
There are two relevant datasets detailing places of worship in the City of Toronto:
- [**City of Toronto's Places of Worship**](csv/opendata_faith.csv) `opendata_faith.csv` from the City of Toronto's [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#4b004922-424b-7860-9e06-2d4fd654daec): this contains a list of faith organizations in Toronto such as churches, mosques, and synagogues. This dataset is current as of 2006 and will not be updated. 
- [**Ontario Heritage Trust's Places of Worship**](csv/heritage_ontario_faith.csv) `heritage_ontario_faith.csv` is sourced from the Ontario Heritage Trust, and is approximately half the size of the City of Toronto's dataset. This dataset is current as of 2012. 

**Format:** Comma Separated Values (CSV)

## Relevance to the Vision Zero Challenge
Places of worship are hubs in the community that attract pedestrian traffic, and may also provide linkages to populations that are at higher risk of being involved in a serious collision. Pedestrians are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and are the focus of a number of existing and planned safety measures.

## Data Dictionary

The format for both datasets are the same:

| Column Name | Type | Description |
|-------------|------|-------------|
ID|Integer| Unique identifier
NAME| Text| The name of the place of worship
POSTAL| Text| Postal code
ADDRESS| Text| Address 
TYPE| Text| Type/denomination/faith of the place of worship
LATITUDE|Float|Latitude
LONGITUDE|Float|Longitude

## Limitations
Note that there is overlap between the two datasets and that both sources are relatively out-of-date. The convention for listing addresses also differs between the two datasets.
