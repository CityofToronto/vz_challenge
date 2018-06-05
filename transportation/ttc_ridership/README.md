# TTC Ridership

## Description
The TTC maintains a dataset, [`ttc_ridership_counts.csv`](csv/ttc_ridership_counts.csv), which contains weekday ridership for all TTC bus and streetcar routes. Each record consists of the total number of boardings and disembarking at each stop, by time period. Each stop is identified by a stop ID detailed in the [TTC Stops](../ttc_stops/) dataset. The dataset was last updated in 2018.

**Format:** Comma Separated Values (CSV)

## Relevance to the Vision Zero Challenge
Transit ridership at individual stops is indicative of pedestrian movements at these locations. Pedestrians are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and is the focus of a number of existing and planned safety measures.

## Data Dictionary
|Column Name|Type|Description|
|:-----|:-----|:-----|
ID|Integer|A unique identifier.
Route|Integer|TTC bus or streetcar route.
COUNT_DATE|Text|Date when the ridership was collected.
Collection Type|Text|Whether the collection is manual or automatic.
Trip Direction|Text|Direction of the leg for the route.
RFP_SEQ_NUM|Integer|Sequential order of stops on each route.
GF_ID|Integer|Stop ID of the stop that can be used with [TTC Stops](../ttc_stops/).
GF_ONST|Text|Street the bus or streetcar is traveling on.
GF_ATST|Text|Cross street that the stop is located at. 
APROVOL_AM|Integer|Total number of riders entering the stop in the AM peak period.
ONS_AM|Integer|Total number of boardings in the AM peak period.
OFFS_AM|Integer|Total number of disembarkings in the AM peak period.
ACCM_AM|Integer|Total number of riders exiting the stop in the AM peak period. 
APROVOL_MD|Integer|Total number of riders entering the stop in the mid-day period.
ONS_MD|Integer|Total number of boardings in the mid-day period.
OFFS_MD|Integer|Total number of disembarkings in the mid-day period.
ACCM_MD|Integer|Total number of riders exiting the stop in the mid-day period.
APROVOL_PM|Integer|Total number of riders entering the stop in the PM peak period.
ONS_PM|Integer|Total number of boardings in the PM peak period.
OFFS_PM|Integer|Total number of disembarkings in the PM peak period.
ACCM_PM|Integer|Total number of riders exiting the stop in the PM peak period.
APROVOL_EE|Integer|Total number of riders entering the stop in the early evening period.
ONS_EE|Integer|Total number of boardings in the early evening period.
OFFS_EE|Integer|Total number of disembarkings in the early evening period.
ACCM_EE|Integer|Total number of riders exiting the stop in the early evening period.
APROVOL_LE|Integer|Total number of riders entering the stop in the late evening period.
ONS_LE|Integer|Total number of boardings in the late evening period.
OFFS_LE|Integer|Total number of disembarkings in the late evening period.
ACCM_LE|Integer|Total number of riders exiting the stop in the late evening period.

**Note:** Fields that are not populated typically indicate that the route is not operational during that time period.

The TTC uses the following definition of time periods for weekday ridership:

|Period|Start Time|End Time|
|:-----|:-----|:-----|
AM Peak|6:00 AM|9:00 AM|
Mid-day|9:00 AM|3:00 PM
PM Peak|3:00 PM|7:00 PM
Early evening|7:00 PM|10:00 PM
Late evening|10:00 PM|1:00 AM

### Limitations
* Some new bus or streetcar routes that have begun service since 2016 may not have ridership data. Additionally, the datasets contains data for routes that have since been terminated.
* Some overnight bus and streetcar services (300 series of routes) have since been renumbered or terminated.
* Additionally, route changes, service changes, or diversions may have been implemented since the count date which may result in different stop locations. 
