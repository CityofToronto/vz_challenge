# Posted Speed Limits

## Description

The City of Toronto Transportation Services maintains [this dataset](tcl_posted_speeds.zip) `tcl_posted_speeds.zip` which contains the posted speed limits on all of the centreline segments from the March 2013 Toronto Centreline. The speed limits are current as of May  2018.

**Format:** ESRI Shapefile

## Relevance to the Vision Zero Challenge

Speed limits define maximum speeds for streets, indicating and enforcing the appropriate speeds for an area to make road users safe. Aggressive driving and distraction is one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and is the focus of a number of existing and planned safety measures. 

### Data Dictionary

|Column Name|Type|Description|
|-----|------|-----|
geo_id | Integer | Unique identifier for centreline segment.
object_id | Integer | System Identifier.
create_id | Integer | Creation ID.
address_l | Text | Range of address numbers on the left side of the street.
address_r | Text | Range of address numbers on the right side of the street.
lf_name | Text | Longform name.
oe_flag_l | Text | Indicates if address numbers on the left side of the street are odd or even.
oe_flag_r | Text | Indicates if address numbers on the right side of the street are odd or even.
fnode | Integer | Intersection ID at the from node.
tnode | Integer | To intersection ID.
lfn_id | Integer | Street name ID.
juris_code | Text | Jurisdiction code.
districtco | Integer | District Number indicating which district is responsible for providing operational services.
str_name | Text | Street name.
str_type | Text | Street type.
str_dir | Text | Street direction.
mar13rc_10 | Integer | Code to represent the 2012 approved City Council Road Classification system.
mar13rc_11 | Text | Description of the 2012 approved City Council Road Classification system.
comment | Text | Comments on speed limit irregularities or errors.
posted_speed | Integer | Posted speed by-law limit based on 2015 and 2016 by-laws. A speed of 1 means that the speed is unavailable.
len_km | Double | Length of segment in kilometres.

### Limitations

The dataset is based on the 2013 Toronto centreline, which is not the most recent version. Where discrepancies exist between the posted speed limit and this GIS layer, observe the limit posted on the street.

There are some entries for which the posted_speed value is a very high value such as '4050' or '3040'. These values occur because different parts of the centreline segment have different speeds. There are approximately 230 rows of data where this issue occurs. 
