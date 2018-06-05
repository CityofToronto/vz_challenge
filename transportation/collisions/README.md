# Collisions

## Description
The Toronto Police Service maintains a database of collisions involving motorized vehicles, cyclists, and pedetrians. These datasets contain information on all recorded collisions between 2008 and 2017.

A collision is defined as the contact resulting from the motion of a motorized vehicle or a streetcar or its load, that produces property damage, injury, or death. For the purposes of this dataset, a collision indicates that the initial point of contact involves at least one motor vehicle or streetcar. 

* The **Events** dataset details unique collisions (or **events**) between vehicles, vehicles and cyclists, vehicles and pedestrians, or vehicles and pedestrians and cyclists. Each record corresponds to a single collision.
* The **Involved** dataset details all individuals involved in the collision, including vehicles, cyclists, and pedestrians. Each record corresponds to a unique individual involved in the collision, with one or more **involved** linked to a specific **event**. This dataset is intended to be used with the **Events** dataset in a one-to-many relationship. 

The datasets are available on an external site:

[Collisions - Events](https://drive.google.com/open?id=1LfaVw2J5RPyofeFuWuYmx5N-ygY5-vHw)

[Collisions - Involved](https://drive.google.com/open?id=1-s9MuY5AxranEp8LyQnjSWKJUfWkHclN)

**Format:** Comma Separated Values (CSV) - semicolon delimited

## Relevance to the Vision Zero Challenge
The datasets show _where_ and _when_ all collisions involving vehicles and other vehicles, cyclists, and pedestrians took place, and includes geographic information and many other collision attributes. This dataset includes collisions involving those that are killed or seriously injured (KSI), the elimination of which is the primary focus of the Vision Zero Road Safety Plan.

## Data Dictionary
**Collisions - Events**

|Column Name|Type|Description|
|-----|-----|-----|
collision_id|Integer|The unique identifier of the dataset, linking this dataset with the `Collisions Involved` dataset. This is not the identifier used by Toronto Police Services, and is unique to this dataset.
collision_date|Date|Date when the collision took place (yyyy-mm-dd).
collision_time|Integer|Time when the collision occurred. Format is in "hhmm".
px|Integer|Primary identifier of all signalized intersection. Please see [Traffic Signals](../traffic_signals/).
street_1|Text|Street/address that the collision occurred on.
street_type_1|Text|Suffix/type of the street.
direction_1|Text|Direction of traffic the collision occurred on.
street_2|Text|Cross-street/address that the collision occurred on.
street_type_2|Text|Suffix/type of the second street.
direction_2|Text|Direction of traffic on the second street that the collision occurred on.
street_3|Text|Third street, if any, the collision occured on.
street_type_3|Text|Suffix/type of the third street.
direction_3|Text|Direction of traffic on the third street that the collision occurred on.
location_class|Text|Class of the location on the road where the collision occurred.
location_desc|Text|Location on the road where the collision occurred.
collision_type|Text|Class/severity of the collision.
impact_type|Text|Type of impact that occurred in the collision.
road_class|Text|Class of road the collision occurred on.
visibility|Text|Visibility conditions at the time and location of the collision.
light|Text|Lighting conditions at the time and location of the collision.
road_surface_cond|Text|Condition of the road surface at the time and location of the collision.
longitude|Numeric|Longitude.
latitude|Numeric|Latitude.

**Collisions - Involved**

|Column Name|Type|Description|
|-----|-----|-----|
collision_id|Integer|Collision unique identifier.
traffic_control|Text|Type of traffic control at the intersection/road (e.g. traffic light, stop sign etc.).
vehicle_class|Text|Class of the vehicle involved in the collision.
initial_dir|Text|Direction the vehicle/cyclist/pedestrian was travelling.
event1|Text|Object/vehicle involved in the collision.
event2|Text|Action the vehicle undertook.
event3|Text|Fixed object involved in the collision.
involved_class|Text|Type of involved individual.
involved_age|Text|Age of involved individual.
involved_injury_class|Text|Level of injury sustained by the individual.
safety_equip_used|Text|Type of safety equipment used by the vehicle.
driver_action|Text|Apparent driver action.
pedestrian_action|Text|Apparent pedestrian action.
pedestrian_collision_type|Text|Categorization of pedestrian collision type.
cyclist_action|Text|Apparent cyclist action.
cyclist_collision_type|Text|Categorization of cyclist collision type.
manoeuver|Text|Vehicle manoeuver.
actual_speed|Text|Actual speed of the vehicle, in kilometers per hour.
posted_speed|Text|Posted speed limit of the road, in kilometers per hour.

**Note**: Most fields will only be populated if applicable/available.

## Limitations

The latitudes and longitudes are generally more reliable than the street fields detailing the intersection that the collision took place. The accuracy of the latitude and longitude, however, is dependent on the user entering the data, and may vary from record to record.
