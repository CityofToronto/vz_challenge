# Dooring Incidents (2014-2017)

## Description

This dataset is a list of all reported dooring incidents to Toronto Police from 2014 to 2017, inclusive. Dooring is defined as an incident in which a cyclist is hit by the door of a motorized vehicle, typically when that door opens onto the path of a cyclist. The file is stored as a comma seperated values (CSV) file, and contains the latitude and longitude (WGS84 projection), the incident date, and the location/intersection of the dooring incident.

## Relevance to the Vision Zero Challenge

This list shows where dangerous vehicular-cyclist interactions occur, which can be used as an indicator for areas with increased incidents, low amounts of warning and safety signage, or adjacent street-side parking and bicycle lanes. 

### Data Dictionary

|Column Name|Type|Description|
|-----|------|-----|
long|Double|Longitude
lat|Double|Latitude
incident_date|Text|The date on which the incident took place (MM/DD/YYYY)
incident_time|Integer|The time at which the incident took place (this is only available between 2014 and 2016) The format of this field is "hhmm" (e.g. 2215 refers to 10:15 PM).
location|Text|Address or intersection at which the incident took place.

### Limitations

Some dooring incidents did not have a specific address recorded. These incidents were coded to the nearest intersection, however, the actual incidents may have took place up to 20m away from the intersection. 
