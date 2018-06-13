# Bluetooth Data

## Description

The City of Toronto Transportation Services maintains these two datasets, [the first](bt_segments.zip) `bt_segments.zip` containing the geography of the Bluetooth sensor segments, and the other `bluetooth_YYYY.csv` containing the travel times along those segments, aggregated into 5 minute bins in individual zipped files for each year. The data is current to June 12th 2018.

**Format:** ESRI Shapefile; Comma Separated Values (CSV)

The data in CSVs are [available on an external site.](https://drive.google.com/open?id=1NeWFW3FYCNEMKUIdK9lsazrzCjuI0xI5)

## Relevance to the Vision Zero Challenge

The Bluetooth data shows the travel times of vehicular travel on certain roads in the downtown core. 

## Data Dictionary

`bt_segments` Shapefile

|Column Name|Type|Description|
|-----------|----|-----------|
|seg_name|Text|Segment name.|
|street|Text|Street or expressway that travel time is being measured.|
|direction|Text|Direction of travel that travel time is measured.|
|start_cross|Text|Intersection that the segment begins at, approximately.|
|end_cross|Text|Intersection that the segment ends at, approximately.|
|length|Integer|Length of the segment.|
|bluetooth|Boolean|Value indicating whether Bluetooth data are used.|
|wifi|Boolean|Value indicating whether WiFi data are used, this is uniquely on expressways.|

`bluetooth_YYYY.csv`

|Column Name|Type|Description|
|-----------|----|-----------|
|segment_name|Text|Segment name.|
|datetime_bin|Timestamp|Time bin indicator in the format of YYYY-MM-DD hh:mm:ss|
|tt|Integer|Travel time of the segment for the given time bin.|
|obs|Integer|Number of observations for the given time bin.|

