# Senior Facilities

## Description
The Transportation Services Division of the City of Toronto compiled [this dataset](senior_facilities.csv) `senior_facilities.csv` for the Vision Zero Challenge, using multiple sources described below.

**Format:** Comma Separated Values (CSV); also available as [GeoJSON](senior_facilities.geojson) and [ESRI Shapefile](senior_facilities.zip)

This is the master dataset of all senior facilities in Toronto. There are two types of facilities listed in this dataset: 
- **Long-term care facilities** are funded by the province and are for seniors that need care at all times. 
- **Retirement homes** are communities or complexes that cater their services to seniors. 

There are seven facilities that are both long term care homes and retirement homes.

Long term care homes were scraped off the Local Health Integration Network website from the following regions:
* [Toronto Central Region](http://www.torontocentralhealthline.ca/listServices.aspx?id=10665)
* [Central Region](http://www.centralhealthline.ca/listServices.aspx?id=10665) 
* [Central East Region](http://www.centraleasthealthline.ca/listServices.aspx?id=10665) 
* [Mississauga Halton Region](http://www.mississaugahaltonhealthline.ca/listServices.aspx?id=10665)

Additional sources included in thie comprehensive dataset include:
* [Long term care homes operated by the City of Toronto](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#c94218ce-0196-ff77-50c4-4eacd8903524)
* [Retirement Homes Regulatory Authority (RHRA) directory](https://www.rhra.ca/en/search-the-public-register/)

The dataset was also supplemented with additional (approximately 10) entries from the [211 directory](https://211ontario.ca/211-topics/older-adults/) for senior facilities.

## Relevance to the Vision Zero Challenge
This dataset provides a list of locations at which a high proportion of the population in the area are likely to be seniors. Older Adults are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and as such are the focus of a number of existing and planned safety measures.

## Data Dictionary
Formatting for both datasets are the same. 

| Column Name | Type | Description |
|-------------|------|-------------|
| ID | Integer | A unique identifier of the facility.  | 
| NAME | Text | The name of the facility. | 
| ADDRESS_OR_INTERSECTION | Text | Street address of the facility.| 
| POSTAL_CODE| Text | Postal code of the facility. | 
| FORMER_MUNICIPALITY	| Text |The former municipality the facility is located in. East York is a separate designation and Toronto is refered to as both *former Toronto* and *Toronto*.  | 
| GC_LATITUDE | Float | Longtitude | 
| GC_LONGITUDE| Float | Latitude | 
| TYPE | Text |  Whether the facility is a long term care home, retirement home, or both | 
