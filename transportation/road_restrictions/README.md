# Road Restrictions

## Description

This dataset is a live feed of current road restrictions/closures and Road Emergency Services Communication Unit (RESCU) incidents in the City of Toronto. [A live map of the Road Restrictions](https://www.toronto.ca/services-payments/streets-parking-transportation/road-restrictions-closures/restrictions-map/) is available.

### Format

The live data feed is available in the following formats from the [Open Data Catalogue](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#fdff6970-e603-c1e8-7d9b-0d08aa6632a9).

<table>
<tbody>
<tr>
<td><strong>Format</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td>XML</td>
<td>Extensible Markup Language (XML) is a common data interchange format.</td>
</tr>
<tr>
<td>XSD</td>
<td>XML Schema Document (XSD) contains information about the XML data structure.</td>
</tr>
<tr>
<td>JSON</td>
<td>JavaScript Object Notation (JSON) is used to load easily into JavaScript enabled web pages.</td>
</tr>
<tr>
<td>JSONP (.json)</td>
<td>Packaged JSON (JSONP) is JSON wrapped in a JavaScript function. JSONP can be reloaded without reloading the page, using the JSON (.json) data extension.</td>
</tr>
<tr>
<td>Timestamp JSON</td>
<td>The Timestamp file is a small file that contains only the timestamp of the most recent update time in the dataset in JSON format.&nbsp; This file can be read quickly to determine if the main data file has changed.</td>
</tr>
<tr>
<td>Timestamp JSONP (.json)</td>
<td>The Timestamp file in JSONP (.json) format.</td>
</tr>
</tbody>
</table>

An archive of Version 2 of the feed is available from 2013 until June 2018 at [`road_restrictions.zip`](road_restrictions.zip) as a Zipped Comma Separated Values (CSV) comma-delimited file.

## Relevance to the Vision Zero Challenge

Road restrictions can identify roadway hazards, areas of increased traffic and collisions that were serious enough that roads remained closed for significant periods of time.

## Data Dictionary

The archive is for Version 2 of the feed and timestamp values have been converted to timestamps with time zones instead of the UNIX epoch found in the live feeds. Consult the [README (`.xls`)](https://www.toronto.ca/ext/open_data/catalog/data_set_files/Road_Restrictions_Readme.xlsx) for the live feeds if you are using those.

| Field                                         | Versions | Type          | Expected Values                                            | Description                                                                                                              |
|-----------------------------------------------|----------|---------------|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| id                                            | 1 and 2  | string        | 'R' or 'I' followed by 5 digits                            | Unique identifier for file.                                                                                              |
| road                                          | 1 and 2  | string        | text                                                       | The name of the road affected.                                                                                           |
| name                                          | 1 and 2  | string        | text                                                       | The name of the closure   containing the road affected and cross street(s).                                               |
| district                                      | 1 and 2  | string        | Etobicoke/ York<br>North   York<br>Toronto/   East York<br>Scarborough| The City District the restriction affects.                                                                               |
| latitude                                      | 1 and 2  | number        | Positive number between   43.000000 and 44.000000          | The latitude where the   restriction is.                                                                                 |
| longitude                                     | 1 and 2  | number        | Negative number between   -79.000000 and -80.000000        | The longitude where the   restriction is.                                                                                |
| roadclass                                     | 1 and 2  | string        | Expressway<br>Expressway   Ramp <br>Major   Arterial <br>Major   Arterial Ramp <br>Minor   Arterial <br>Minor   Arterial Ramp <br>Collector <br>Local <br>Other <br> | The class of road the restriction is on.                                                                                 |
planned                                       | 1 and 2  | unsigned byte | 1 or 0                                                     | 1 if the restriction is planned   and 0 if not.                                                                          |
| severity_override                              | 1 and 2  | unsigned byte | 1 or 0                                                     | 1 if the impact of the   restriction is greater than expected for the time of day and roadclass and 0   if not.          |
| source                                        | 1 and 2  | string        | RESCU<br>Media<br>Public<br>911<br>EMS<br>Fire<br>DOC<br>Police<br>| How the traffic centre found out about this   restriction.                                                               |
| created_time                               | 2        | timestamp | Timestamp at the Toronto time zone in the format: <br>`YYYY-MM-DD HH24:Min:Sec` | The timestamp marking when the   restriction record was created.                                                         |
| last_updated                                   | 1 and 2  | timestamp | Timestamp at the Toronto time zone in the format: <br>`YYYY-MM-DD HH24:Min:Sec` | The timestamp of the last change   to the restriction record.                                                            |
| start_time                                     | 1 and 2  | timestamp | Timestamp at the Toronto time zone in the format: <br>`YYYY-MM-DD HH24:Min:Sec` | The timestamp when the   restriction is expected to start.                                                                |
| end_time                                       | 1 and 2  | timestamp | Timestamp at the Toronto time zone in the format: <br>`YYYY-MM-DD HH24:Min:Sec` | The timestamp when the   restriction is expected to end.                                                                 |
| work_period                                    | 1 and 2  | string        | Daily<br>Weekdays<br>Weekends<br>Continuous| The days of week when the restriction is   expected to be in place.                                                      |
| expired                                       | 1 and 2  | unsigned byte | 1 or 0                                                     | Indicates if the restriction has   expired.                                                                               |
| signing                                       | 1 and 2  | string        | text                                                       | Any sign messages that were on   changeable message sign in relation to this restriction.                                |
| notification                                  | 1 and 2  | string        | text                                                       | Agencies contacted in relation   to this restriction.                                                                     |
| work_event_type                                 | 1 and 2  | string        | Construction<br>Maintenance<br>Utility   Cut<br>Special   Event<br>Filming   Parade<br>Demonstration<br>Other| The type of work or event that is causing the   restriction.                                                             |
| contractor                                    | 1 and 2  | string        | text                                                       | The contractor who has requested   the restriction.                                                                      |
| permit_type                                    | 1 and 2  | string        | RACS<br>Street   Event<br>Film<br>Other| The type of permit issued for the restriction.|
| tescription                                   | 1 and 2  | string        | text                                                       | A description of the   circumstances surrounding the restriction.                                                        |
| special_event                               | 1 and 2  | string        | Yes or No                                                  | Is the restriction related to a   special event.                                                                         |
| from_road                                      | 2        | string        | text                                                       | The road at the beginning of a   restriction zone.                                                                       |
| to_road                                        | 2        | string        | text                                                       | The road at the end of a   restriction zone.                                                                             |
| at_road                                        | 2        | string        | text                                                       | The cross road of a restriction.                                                                                          |
| direction                            | 2        | string        | BOTH_DIRECTIONS <br> ONE_DIRECTION| How many directions are affected.|
| type                                          | 2        | string        | ACCIDENT<br>HAZARD<br>CONSTRUCTION<br>ROAD_CLOSED| Type of restriction. |
| subtype                                       | 2        | string        | Type=ACCIDENT [ACCIDENT_MAJOR]<br>Type=ACCIDENT   [ACCIDENT_MINOR]             <br>Type=ROAD_CLOSED   [ROAD_CLOSED_EVENT]       <br>Type=ROAD_CLOSED   [ROAD_CLOSED_CONSTRUCTION]<br>Type=ROAD_CLOSED   [ROAD_CLOSED_HAZARD]| Sub type of restriction.|
| schedule_monday                                | 2        | string        | HH:MM-HH:MM or   <br>HH:MM-24:00,00:00-HH:MM                                            | The times of day on Mondays that the restriction   is active.                                                              |
| schedule_tuesday                               | 2        | string        | HH:MM-HH:MM or  <br>HH:MM-24:00,00:00-HH:MM                                          | The times of day on Tuesdays that the   restriction is active.                                                             |
| schedule_wednesday                             | 2        | string        | HH:MM-HH:MM or <br>HH:MM-24:00,00:00-HH:MM | The times of day on Wednesdays that the   restriction is active.                                                           |
| schedule_thursday                              | 2        | string        | HH:MM-HH:MM or <br>HH:MM-24:00,00:00-HH:MM | The times of day on Thursdays that the   restriction is active.                                                            |
| schedule_friday                                | 2        | string        | HH:MM-HH:MM or <br>HH:MM-24:00,00:00-HH:MM | The times of day on Fridays that the restriction   is active.                                                              |
| schedule_saturday                              | 2        | string        | HH:MM-HH:MM or <br>HH:MM-24:00,00:00-HH:MM | The times of day on Saturdays that the   restriction is active.                                                            |
| schedule_sunday                                | 2        | string        | HH:MM-HH:MM or <br>HH:MM-24:00,00:00-HH:MM | The times of day on sundays that the restriction   is active.                                                              |
| schedule_everyday                              | 2        | string        | HH:MM-HH:MM or <br>HH:MM-24:00,00:00-HH:MM | The times of day everyday that the restriction   is active.                                                                |
| geo_polyline                                   | 2        | string        | [[latitude,longitude],[latitude,longitude],…]              | A list of coordinates in WGS84   latitude/ longitude pairs that represent the affected road in the affected   direction. |

## Limitations

Planned work doesn't necessarily take place during the full period listed; it only reflects the period of dates/times when work is **permitted**.
