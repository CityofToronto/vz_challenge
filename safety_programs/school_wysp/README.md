# School - Watch Your Speed (WYS) Signs

## Description


The City of Toronto's Transportation Services Division maintains a listing [(`school_wysp.zip`)](csv/school_wysp.zip) of the locations of radar speed display signs, deployed as part of the "Watch Your Speed" Program in school zones. These signs were installed with the goal of reducing speeds in areas with heavy populations of young children. This dataset was last updated in March 2018.

**Format:** ESRI Shapefile (NAD27)

## Relevance to the Vision Zero Challenge 

The deployment of "Watch Your Speed" signs is a key safety measure used to enhance the safety of School Children, one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan.

## Data Dictionary 
| Column Name | Type | Description |
|-------------|------|-------------|
Num | Integer | Unique Identifier
School_Nam | Text | Full name of the school
Type | Text | Program type (either Existing Pilot Project or New)
Speed_Sign | Text | Date on which sign was installed (DD-MMM-YY)
Street | Text | Street on which sign was installed
Direction | Text | Cardinal direction of traffic
Side_of_St | Text | Side of street on which sign was installed
Location | Text | Street address where sign was installed
LAT | Float | Latitude, NAD27
LONG | Float | Longitude, NAD27

