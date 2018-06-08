# Traffic Signals

## Description
The City of Toronto's Transportation Services Division maintains lists of all traffic signals, flashing beacons, and pedestrian crossovers within the City of Toronto, including their locations. These datasets also include related operational characteristics, such as the type of system and the date the signal was activated.

Additionally, these datasets include information on safety programs (APS, UPS, LPI, and Bicycle signals) installed at each signal:

 - A **Accessible Pedestrian Signal (APS)** provides visually impaired pedestrians an audible signal to cross the intersection. [More info](https://www.toronto.ca/services-payments/streets-parking-transportation/traffic-management/traffic-signals-street-signs/types-of-traffic-signals/accessible-pedestrian-signals/)
 - A **Leading Pedestrian Interval (LPI)** allows pedestrians to start crossing the intersection before vehicles are given the signal to move. This gives pedestrians more visibility within the intersection and improves motorist yielding behaviour towards pedestrians in a crosswalk. [More info](https://www.toronto.ca/services-payments/streets-parking-transportation/traffic-management/traffic-signals-street-signs/types-of-traffic-signals/leading-pedestrian-interval-phase/)
 - An **Uninterruptible Power Supply (UPS)** ensures the traffic light continues to operate in the event of a loss in power. Bicycle Signals control cyclist's movement in an intersection separate from pedestrian or vehicle signals. 

**Format:** Comma Separated Values (CSV); JavaScript Object Notation (JSON); Extensible Markup Language (XML)

The datasets are available on the City of Toronto's [Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#6899bafa-1ffb-faaa-3bb2-7d2eac794205).

## Relevance to the Vision Zero Challenge
Signalized intersections and pedestrian crossovers (PXOs) are key components of the City of Toronto's transportation network. These intersections are the base layer on which transportation infrastructure is built, and against which many transportation datasets are referenced.

Additionally, this dataset gives information on four safety programs (APS, UPS, LPI, and Bicycle signals) that aim to protect pedestrians and cyclists who are 2 of the 6 emphasis areas in the Vision Zero Road Safety Plan.

## Data Dictionary

Some columns in the table below are not present in version 1 of the data.

| Column Name | Type | Description |
|-------------|------|-------------|
PX| Integer | 1 <= PX <= 4999 
MAIN| Text | Main Street
MIDBLOCK| Text | Distance to nearest side street (device not located at an intersection)
SIDE1| Text | Side 1 Street
SIDE2 | Text | Side 2 Street
PRIVATE_ACCESS | Text | A driveway, laneway, entrance, etc.
ADDITIONAL_INFO | Text | Other related information
GeoID| Integer | End Node Identifier
NODEID| Integer | Intersection Node Identifier
X| Integer | Easting 
Y | Integer | Northing
Latitude | Numeric | 
Longitude | Numeric | 
ACTIVATION_DATE | Date | Date when signal was installed and put in operation (YYYY/MM/DD)
SIGNAL_SYSTEM | Text | MTSS, SCOOT, TransSuite, Aries, or Awaiting TransSuite
NON_SYSTEM | Text | Signal not connected to a central system  (value=local or temporary)
MODE_OF_CONTROL | Text | FXT, SAP, SAP on Recall, SAV, SA2, PED
Pedestrian Walk speed | Text | Designed walk speed in meters per second
APS| Integer | Enable with sound (=1), Not installed (=0)
APS Operation | Text | [Fixed time, Pushbutton]
APSACTIVATIONDATE | Date | The date that APS was activated for this location, where applicable.
TRANSIT_PREEMPT| Integer | The signal has (yes=1,no=0) a feature that pre-empts it for transit vehicles
FIRE_PREEMPT| Integer | The signal has (yes=1,no=0) a feature that pre-empts it for firehall vehicles
RAIL_PREEMPT| Integer | The signal has (yes=1,no=0) a feature that pre-empts it for railway trains
NO_OF_SIGNALIZED_APPROACHES| Integer | number of vehicle approaches to a signalized intersection.
UPS | Integer | (1=yes, 0=no) indicates this location has backup power.
LEDBLANKOUTSIGN | Integer | (1=yes, 0=no) indicates this location has signage that can be turned on or off i.e. time of day turn prohibitions.
LEADINGPEDESTRIANINTERVAL | Integer | (1=yes, 0=no) indicates this location has signal timings that allow pedestrian movement before vehicular movement.
BICYCLESIGNAL - (1=yes, 0=no) indicates this location has signal specifically heads for bicycle traffic.

