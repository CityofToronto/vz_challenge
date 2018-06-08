# Red Light Camera (RLC) Infractions

## Description

The City of Toronto Transportation Services maintains a dataset of the number of infractions at all red light cameras by year. Red light cameras automatically capture a photo of any vehicle entering the intersection after the signal changes to a red light. More information can be found [here](https://www.toronto.ca/311/knowledgebase/kb/docs/articles/transportation-services/transportation-infrastructure-management/operational-planning-and-policy/operational-planning-and-policy/red-light-cameras.html) and [here](https://www.toronto.ca/services-payments/streets-parking-transportation/traffic-management/pavement-markings/red-light-cameras/). The data is up to date to 2017.

**Format:** Comma Separated Values (CSV)

## Relevance to the Vision Zero Challenge

Red light cameras are an enforcement measure that deters vehicles from entering and blocking the intersection during a red light. This program addresses distracted and aggressive driving, which is one of six emphasis groups outlined in the Vision Zero Road Safety Plan. 

## Data Dictionary

|Column Name|Type|Description|
|:------|:------|:------|
Intersection|Text|Name of the streets at the intersection.
PX|Integer|Traffic Signal identifier used by Transportation Services. This identifier is common with the `traffic_signals` dataset found [here](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#6899bafa-1ffb-faaa-3bb2-7d2eac794205).
year|Integer|Year.
infractions|Integer|Number of infractions in the given year.

## Limitations

A blank entry or an entry with a value of 0 in the `infractions` column may indicate that the red light camera was not operational or not installed during that year.
