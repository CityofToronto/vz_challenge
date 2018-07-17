# Pavement Width and Number of Lanes 

## Description 
This dataset contains information about the pavement width and number of lanes in the City of Toronto. 
The dataset such as the pavement width and number of lanes is current as of 2012. However, the data is overlaid on the 
2014 Toronto Centreline.

**Format:** ESRI Shapefile (UTM)

## Relevance to the Vision Zero Challenge
This dataset provides additional information about roadways, such as their widths. 

## Data Dictionary 

| Column Name | Type | Description |
|-------------|------|-------------|
OBJECTID * | ObjectID | Unique ID
GEO_ID | Long | Geographic ID
FromStreet | String | Street Name at Segment Start
ToStreet | String | Street Name at Segment End
MAR13RC2012_RENDER_DESC | String | Road Classification Description
NumberofLa |Long | Number of Through Lanes
Width | Short | Pavement Width - curb to curb
SHAPE | Geometry |Shape Type
SHAPE_Length | Double |Associated Segment Length
Section_ID | String | Segment ID
Length | Double |Associated Street Length
LF_NAME | String | Road Name
MAR13RC2012_FCODE |  Long | TCL Feature Code
MAR13RC2012_FCODE_DESC | String |TCL Feature Code Description
MAR13RC2012_RENDER | Long |Road Classification Code
MAR13RC2012_JURIS | String |Road Jurisdiction
GIS_ROUTE | Double | GIS Route Number


## Limitations
The dataset is not current, as it is from 2012. The version of the Toronto Centreline layer that the data is overlaid on is from 2014. 
