# Transit Shelters

## Description
The City of Toronto Street Furniture Program maintains [this dataset](SFM_transit_shelters.zip) `SFM_transit_shelters.zip`, which contains all of the transit shelters in Toronto for bus and streetcar surface routes. All shelters have the ability to support advertisements.

The data was last updated in 2018, and is in the MTM 3 Degree Zone 10 NAD27 coordinate reference system. 

**Format:** ESRI Shapefile (NAD27)

## Relevance to the Vision Zero Challenge
Transit shelters are part of a safety program to protect transit users from road traffic and environmental conditions. Pedestrians are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and is the focus of a number of existing and planned safety measures.

## Data Dictionary
|Column Name|Type|Description|
|-----|-----|-----|
Object ID|Integer|A unique identifier.
ASSETID|Text|A unique identifier used by Transportation Services.
ID|Text|Same as ASSETID
ADDRESSNUM|Integer|Address number that the shelter is closest to.
ADDRESSTR|Text|Street that the shelter is on
SITEID|Text|A unique identifier for the site used by Transportation Services.
WARD|Integer|Ward number the shelter is located in.
FRONTINGST|Text|Street that the shelter serves.
SIDE|Text|Which side of the fronting street the shelter is on.
FROMSTREEET|Text|Cross street of the intersection the shelter is on.
DIRECTION|Text|Direction the transit route is moving.
BIA|Text|Business improvement association the shelter is located in.
ASSETTYPE|Text|Type of shelter.
STATUS|Text|Whether the shelter needs to be removed or temporarily removed.
STYLE|Text|Manufacturer/model of the shelter.
POSTERBOAR|Text|Whether the shelter has a poster board for TTC information.
POSTERBO_1|Text|The status of the poster board.

## Limitations 

Due to construction and other factors, the list can vary by between 2-5% at any time.
