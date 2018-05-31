# HERE Probe Speeds

### Description

The City of Toronto [purchases](https://360.here.com/2017/05/11/here-helps-toronto-take-data-driven-approach-transport-management/) real-time and archived traffic speed data from [HERE](https://www.here.com/en/products-services/here-traffic-suite/here-traffic-overview) a mapping and navigation company. These data are collected from "probes"&mdash;a proprietary mix of connected cars, commercial fleets, and navigation app users&mdash;over the entire City of Toronto and aggregated into five minute bins. This dataset provides a distribution of observed speeds on links for business days during the September to November period in 2017.

The speeds are aggregated on a per-probe basis, not a per-vehicle basis, in order to capture greater variability in speeds along a link. This means that some observations can be affected by traffic signals or stop signs. This does also mean that some amount of speeding along any link can be captured.

**Format:** Comma Separated Values (CSV); ESRI Shapefile

### Relevance to the Vision Zero Challenge

Speed is directly related to the severity of collisions, and the seriousness of injury or likelihood of death. Speeding in excess of the speed limit is considered aggressive driving and increases likelihood of a crash. This dataset can indicate where design interventions should be made to discourage speeding.

### Data Dictionary

**Note on link definitions**: Links are defined by a reference node, and a non-reference node. The reference node is always the node with the lowest latitude, in the case of two nodes with equal latitude, the node with the lowest longitude is the reference node. 
Speeds are referenced to a link-direction combination `link_dir`, whereas the geography is defined by unique links.  `link_id`s can be joined to the `link_dir` by removing the final character from `link_dir` e.g. in SQL `link_id = LEFT(link_dir, -1)::numeric`

#### Speed distributions

| Column Name | Type | Description |
|-------------|------|-------------|
|link_dir     |Text| This uniquely identifies a link with a number representing the segment followed by a letter (F, T) indicating whether the direction of travel if From or Towards the Reference Node (see **note** above) |
|Hour   |Time|The hour of business day over which the observations are aggregated|
|spdlimit     |Integer| The speed limit on that segment, as collected by HERE |
|pct      |Integer| The percentage of observations with equivalent or lesser speed to the `speed` column |
|speed    |Integer| The speed for this percentile for this `hour` and `link_dir` |

#### Streets geography

| Column Name | Type | Description |
|-------------|------|-------------|
|link_id | Integer | Unique id for links. See **note** above for information about joining. |
|st_name | Text | Street Name |
| dir_travel | One character | Indicates allowed directions of travel on this street `B` for Both, `T` for towards the reference node, and `F` for from the reference node. |

### Limitations

Because speeds are aggregated on a per-observation basis of a sample of vehicles, it would be incorrect to refer to the percentiles as a percentage of vehicles travelling on the link for that hour. Furthermore, unlike [Speed Counts](../SpeedVolumes/) which are taken at a fixed location, the locations of observations could be anywhere along a link so the power of comparing different percentiles along a given link.

Sample sizes can be limited for smaller streets in the City.

The speed limit information is collected by HERE. When discrepancies exist between the posted speed limit and the speed limit in this dataset, the posted speed limit should be considered accurate.

Nevertheless we think this is a useful set of data to identify where and when speeding occurs (and can occur) across the City.
