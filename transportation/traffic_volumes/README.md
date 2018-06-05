# Traffic Volumes

## Description
The City of Toronto's Transportation Services Division collects traffic volume data across the city from a variety of sources for a number of purposes. This data generally takes one of two forms:

1. **Automatic Traffic Recorders (ATR) Counts:** Segment-level volumes reflecting the total number of observed vehicles on a specific street moving in a specific direction(e.g. the total number of vehicles observed on King St. heading Eastbound, just west of Spadina Ave.)
2. **Turning Movement Counts (TMCs):** Movements observed at a specific intersection, typically indicating the total number of vehicles observed at each leg (i.e. North, South, East, or West) of the intersection and, if applicable, the observed turning movement (i.e. Through, Left Turn, or Right Turn), by mode (e.g. the total number of vehicles observed at the South leg of King and Spadina, turning right).

The datasets available in this repository are a curated collection of these counts, and are separated into four distinct datasets):
* **Turning Movement Counts (TMCs) - Permanent**: Volumes observed at intersections across the city, by turning movement and mode, at permanent counting stations.
* **Turning Movement Counts (TMCs) - Short Term**: Volumes observed at intersections across the city, by turning movement and mode, at short-term counting stations.
* **Automatic Traffic Recorders (ATR) Counts - Permanent**: Volumes observed on specific streets, by direction and mode, at permanent counting stations.
* **Automatic Traffic Recorders (ATR) Counts - Short Term**: Volumes observed on specific streets, by direction and mode, at short-term counting stations.

The datasets are available on an external site:
1. [Turning Movement Counts (TMCs) - Permanent](https://drive.google.com/open?id=1AY-tSutw3q0gYFfDCSWjKHd1eQQwI9Xm)
2. [Turning Movement Counts (TMCs) - Short Term](https://drive.google.com/open?id=17HrXgTWCVrcj4imjwW08KZEvpE-wgxBk)
3. [Automatic Traffic Recorders (ATRs) - Permanent](https://drive.google.com/open?id=1uMcISQ3nQ4_22xFhv5QuC9QDjZt7c6JO)
4. [Automatic Traffic Recorders (ATRs) - Short Term](https://drive.google.com/open?id=1l-lHqT4hVhN1dL8zaR7KHWUpsjfiftXs)

### Relevant Spatial Linkages
**Turning Movement Counts (TMCs)** have been tagged to specific [traffic signals](../traffic_signals/).

**Automatic Traffic Recorder (ATR) Counts** have been tagged to specific streets as defined by the City's [Centreline](../toronto_centreline/).

**Format:** Comma Separated Values (CSV) - semicolon delimited

## Relevance to the Vision Zero Challenge

Traffic volumes are typically one of the key drivers for a number of transportation infrastructure decisions, such as the decision to create a signalized intersection, or to optimize traffic signal timings. This data can be used to identify which streets on the city's road network experience high volumes of traffic, and which times of the day are the busiest.

These datasets also include both pedestrian and cyclists volumes, where available. Pedestrians and Cyclists are two of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and as such are the focus of a number of existing and planned safety measures.

## Data Dictionary

**Turning Movement Counts (TMCs)**

| Column Name | Type | Description |
|-------------|------|-------------|
| px  | Integer | Signalized intersection identifier linking back to the City's Traffic Signals dataset. |
| location | Text | Textual description of street segment location and direction. |
| class_type | Text | Textual description of the modal class (Cyclists, Pedestrians, or Vehicles). |
| leg | Text | Textual description of the specific leg of the intersection (N, S, E, or W). |
| movement | Text | Textual description of the specific movement observed (Through, Left, or Right). If NULL, record represents volumes observed on the crosswalk. |
| datetime_bin | Timestamp | Start of 15-minute period. |
| volume_15min | Integer | Total volume observed over the 15-minute period. |


**Automatic Traffic Recorders (ATRs)**

| Column Name | Type | Description |
|-------------|------|-------------|
| centreline_id  | Integer | Street segment identifier linking back to the City's Centreline. | 
| direction | Text | Cardinal direction of vehicle travel along street segment. | 
| location | Text | Textual description of street segment location and direction. | 
| class_type | Text | Textual description of the modal class (Cyclists, Pedestrians, or Vehicles). |
| datetime_bin | Timestamp | Start of specific period. |
| resolution | Timestamp | Size of temporal period (typically 15 minutes or 1 hour). |
| volume_15min | Integer | Total volume observed over the specific period. |
