# Speed-Volume Counts

## Description
The City of Toronto's Transportation Services Division collects volume data in 15-minute intervals at locations across its network, along with the measured speed of each of these individual vehicles in predefined speed bins. These counts are typically collected over one- or three-day periods (although there are instances that break from this general rule).

This data is provided in two distinct forms:
* **Disaggregate**: Total 15-minute volumes observed at each location, by speed bin.
* **Summarized**: Estimated median, 85th percentile, and 95th percentile speeds at each location, by day.

The summarized dataset is derived directly from the disaggregate dataset and is estimated by interpolating (assuming a uniform distribution) within the predefined speed bin. 

The datasets are available on an external site:

[Speed Volumes - Disaggregate](https://drive.google.com/open?id=1Mdo7u2vhDnjxU5bvk43KxjRT2h2As9NA)

[Speed Volumes - Summarized](https://drive.google.com/open?id=1Jh4ps1HTJzfrZb7tYeAJ-EdQYkGnEb9K)

#### Aggregation Example
A total of 1000 cars are counted on a specific day at a specific location, the 85th percentile speed is set to the estimated speed of the 850th car (when ordered by speed). If 750 cumulative cars are counted within speed bins below 50 kilometers per hour (kph), and 900 cumulative cars are counted within speed bins below 55 kph, the 85th percentile speed is estimated to be 50 kph + (55 kph - 50 kph) * (850 cars - 750 cars) / (900 cars - 750 cars) = 53.33 kph. If specific percentile speeds are estimated to be less than 19 kph or greater than 80 kph, an exact value is not provided.

The speed bin definitions are as follows:

| Speed Bin | Speed Range, in kph |
|-----------|---------------------|
| 1 | [0,19) |
| 2 | [19,25) |
| 3 | [25,30) |
| 4 | [30,35) |
| 5 | [35,40) |
| 6 | [40,45) |
| 7 | [45,50) |
| 8 | [50,55) |
| 9 | [55,60) |
| 10 | [60,65) |
| 11 | [65,70) |
| 12 | [70,75) |
| 13 | [75,80) |
| 14 | [80,Inf) |


## Relevance to the Vision Zero Challenge

This dataset provides the speed distribution at a diverse set of locations across the city. This can help identify where speeding issues may be present and/or evaluate the effectiveness of traffic calming measures.

## Data Dictionary

**Speed Volumes - Disaggregate**

| Column Name | Type | Description |
|-------------|------|-------------|
| centreline_id  | Integer | Street segment identifier linking back to the City's Centreline | 
| direction | Text | Cardinal direction of vehicle travel along street segment | 
| location | Text | Textual description of street segment location and direction | 
| datetime_bin | Timestamp | Start of 15-minute period |
| speed_kph | Integer Range | Start and end of speed bin, in kilometers per hour (kph) |
| volume_15min | Integer | Total volume observed within speed bin over the 15-minute period |


**Speed Volumes - Summarized**

| Column Name | Type | Description |
|-------------|------|-------------|
| centreline_id  | Integer | Street segment identifier linking back to the City's Centreline | 
| direction | Text | Cardinal direction of vehicle travel along street segment | 
| location | Text | Textual description of street segment location and direction | 
| dt | Date | Date during which counts were conducted |
| speed_kph_50 | Text | Estimated median speed over full day, in kilometers per hour (kph) |
| speed_kph_85 | Text | Estimated 85th percentile speed over full day, in kilometers per hour (kph) |
| speed_kph_95 | Text | Estimated 95th percentile speed over full day, in kilometers per hour (kph) |
