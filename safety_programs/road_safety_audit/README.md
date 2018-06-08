# Road Safety Audit

## Description
The City of Toronto Transportation Services maintains [this dataset](road_safety_audit.zip), `road_safety_audit.zip`,  of the location and length of road safety audits conducted by City of Toronto Transportation Services in 2017. As part of the the Vision Zero Road Safety Plan, these in-depth safety reviews were conducted in areas with high Killed of Seriously Injured (KSI) collisions in order to identify immediate deficiencies and issues and determine appropriate short-term and long-term remedial actions. 

**Format:** ESRI Shapefile (WGS84)

## Relevance to the Vision Zero Challenge
As part of the the Vision Zero Road Safety Plan, the road safety audits were conducted in areas with high KSI collisions in order to identify immediate deficiencies and issues and determine appropriate short-term and long-term remedial actions. 

## Data Dictionary
|Column Name|Type|Description|
|:-----|:-----|:-----|
Id|Integer|A unique identifier. There may be duplicate entries since one road safety audit can span over multiple road segments on the Toronto centreline file.
Length|Integer|Length of the road safety audit study area. There may be duplicate entries since one road safety audit can span over multiple road segments on the Toronto centreline file.
geo_id|Integer|Centreline ID that the road segment corresponds to on the Toronto centreline file.

