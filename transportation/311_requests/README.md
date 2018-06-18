# 311 Requests

## Description
The dataset contains information on customer initiated service requests received by 311 Toronto. This data was collected from multiple channels including telephone, fax, email, online self-serve requests, mobile API and Twitter.

311 manages City divisional service request data for Solid Waste Management, Transportation Services, Toronto Water, Municipal Licensing & Standards, and Urban Forestry. 311 consulted with these participating divisions and subject matter experts for this dataset release.

**Format:** Comma-Separate Value (CSV)

The dataset is zipped and available on the [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#2fc027de-d27a-2a00-1388-6849497cb84c).

## Relevance to the Vision Zero Challenge
The following `Service Request Type` may indicate requests for safety improvements or demand for accessible facilities:

- Complaint-Access
- Complaint-Disability
- Disabled Persons' Parking Space
- New Pedestrian Crossover
- New Traffic Control Signal Request
- Pedestrian Crossing Protection
- Pedestrian Crossover Operation
- Pedestrian Issues/Timing/Delays
- Pedestrian Refuge Island
- PXO Maintenance

## Data Dictionary

| Field /   Column Name | Description /   Definition | Comments /   Example |
|-----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------|
| Service Request Creation Date and Time  | The   date and time when a service request (SR) is created and submitted into a   work management system of a respective Service Request Division. | 01/Jan/2017 12:10 AM |
| Service Request Location  | The   readable description of location recorded for the service request. The   location is recorded as the first three characters of the postal code of the   service request (forward sortation area: FSA), or the street intersection of   the location of the service request. The Open Data set only shows SRs which   are validated in the City's GeoSpatial system. Such SRs would have either   street address or intersection specified as a location. | M9A |
| Original Service Request Type  | The   readable name of the service request type also known as problem code name   created by 311 Toronto on behalf of the customer. The 311 Contact Centre   creates the request which is transmitted to the appropriate City division for   action. | Noise |
| Service Request Status  | The   current status of the service request:     <br>- **Initiated** - The service   request has been received and assigned to the appropriate City division for   review and action.     <br>- **In Progress** - The   assigned City division is currently working on resolving the service   request. <br>- **Canceled** - A   service request is cancelled for one of several reasons i.e., call is   disconnected, caller doesn't wish to create the SR, caller calls back to   cancel the request or the SR is created in error, etc. <br>- **Closed** - The   appropriate City division has investigated the customer concern and has taken   the necessary action to resolve the request. | Closed |
| Service Request Division  | Represents   the responsible 311 Integrated Service Division. Division shown in the Open   Data shall correspond to the original SR type, regardless of subsequent SR   type changes by the back-end divisions. | Municipal   Licensing & Standards |
| Service Request Section-Unit  | Represents   the section or unit within the responsible 311 Integrated Service Division. | District   Enforcement |
| Service Request Ward  | Represents   the readable description of the electoral ward name and number recorded for   the service request. The Open Data System will display ward as follows: `Ward Name (Ward Number)`.     | Etobicoke   Centre (04) |

## Limitations
Each request requires evaluation and in its own does not indicate that there was a safety issue.

A status of **Closed** does not necessarily indicate that an action was taken.
