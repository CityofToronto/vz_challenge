# Crossing Guard Location

## Description

List of every intersection where there is a crossing guard to aid children and people crossing the road. Data is sourced internally from the Traffic Safety Unit, City of Toronto and is current as of 2017.

## Relevance to the Vision Zero Challenge

This data can help assess which parts of the city already have safety measures in place to prevent vehicular incidents with children, an at-risk group of the population.

## Data Dictionary

The format of this file is a shapefile that can be opened using GIS software.

| Column Name | Type | Description |
|-------------|------|-------------|
wkt_geom  | Float | Coordinates in XY format
Location | Text | Unique Identifier
Main_St|Text|The primary road at the intersection
Cross_St|Text|The secondary road at the intersection
Toronto_Di|Text|The TCDSB school this crossing guard serves
Toronto_1|Text|The TDSB school this crossing guard serves
Remove|Text|Date that crossing guards were removed
Type|Text|Type of intersection. PXO refers to pedestrian crossing
District|Text|The district (Etobicoke, Scarborough, North York, Toronto and East York) the crossing guard is located in
