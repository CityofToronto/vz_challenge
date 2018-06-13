# Dooring Incidents (2014-2017)

## Description

Toronto Police maintains [this dataset](dooring_14_17.csv) `dooring_14_17.csv` of all cyclist dooring incidents reported to Toronto Police from 2014 to 2017, inclusive. The file contains the latitude and longitude (WGS84 projection), the incident date, the incident time (for incidents prior to 2017) and the location/intersection of the dooring incident.

Dooring is defined as an incident in which a cyclist is hit by the door of a motorized vehicle, typically when that door opens onto the path of a cyclist. Since 2013, dooring collisions have not been considered a Motor Vehicle Collision by the Ministry of Transportation and as a result are not including in Motor Vehicle Collision Reports filed by the Toronto Police Service.

**Format:** Comma Separated Values (CSV)

## Relevance to the Vision Zero Challenge

Dooring incidents are an important safety concern for cyclists in the City of Toronto and is a common challenge on downtown arterials with on-street parking, in particular when combined with streetcar routes. Cyclists are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and is the focus of a number of existing and planned safety measures.

### Data Dictionary

|Column Name|Type|Description|
|-----|------|-----|
long|Double|Longitude
lat|Double|Latitude
incident_date|Text|The date of the incident (MM/DD/YYYY)
incident_time|Integer|The time of the incident (this is only available between 2014 and 2016) The format of this field is "hhmm" (e.g. 2215 refers to 10:15 PM).
location|Text|Address or intersection at which the incident took place.

### Limitations

Some dooring incidents did not have a specific address recorded. These incidents were coded to the nearest intersection, however, the actual incidents may have taken place up to 20m away from the intersection. 
