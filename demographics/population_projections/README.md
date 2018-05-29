# Population Projections

## Description
Annual population projections, from 2017 to 2041.

These population projections are organized among 4 different datasets:
* projections for the whole province
* projections for each census division
* projections for each Local Health Integration Network (LHIN)
* projections for each Ministry of Children and Youth Services’ Service Delivery Division (SDD) region

Each dataset includes population projections by age and gender, and are in Excel (xlsx) format.

These datasets are owned by the Ministry of Finance, and were last modified on June 1, 2017. They can be found on the Government of Ontario's [Open Data Catalogue](https://www.ontario.ca/data/population-projections).

## Relevance to the Vision Zero Challenge
These projections can help inform where changes to population demographics are likely to occur, specifically those with ties to the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan.

## Data Dictionary 

### Provincial Projections by Age and Sex, 2017-2041
| Column Name | Type | Description |
|-------------|------|-------------|
Year (July 1) | Integer | Year that the population projections in the current row are for
SEX | Text | Sex 
0 | Integer | Projected number of people in Ontario with the age of 0
1 | Integer | Projected number of people in Ontario with the age of 1
....
90+ | Integer | Projected number of people in Ontario that are 90 years old or greater

### Census Division Projections  by Age and Sex, 2017-2041
| Column Name | Type | Description |
|-------------|------|-------------|
Year (July 1) | Integer | Year that the population projections in the current row are for
REGION CODE | Integer | Census Division code
REGION NAME | Text | Census Division name
SEX | Text | Sex 
0 | Integer | Projected number of people in census division with the age of 0
1 | Integer | Projected number of people in census division with the age of 1
....
90+ | Integer | Projected number of people in census division that are 90 years old or greater

### Local Health Integration Networks (LHINs) Projections by Age and Sex, 2017-2041
| Column Name | Type | Description |
|-------------|------|-------------|
Year (July 1) | Integer | Year that the population projections in the current row are for
REGION CODE | Integer | LHIN code
REGION NAME | Text | LHIN name
SEX | Text | Sex 
0 | Integer | Projected number of people in LHIN with the age of 0
1 | Integer | Projected number of people in LHIN with the age of 1
....
90+ | Integer | Projected number of people in LHIN that are 90 years old or greater

### Ministry of Children and Youth Services’ Service Delivery Division (SDD) region Projections by Age and Sex, 2017-2041
| Column Name | Type | Description |
|-------------|------|-------------|
Year (July 1) | Integer | Year that the population projections in the current row are for
REGION CODE | Integer | Service Delivery Division code
REGION NAME | Text | Service Delivery Division name
SEX | Text | Sex 
0 | Integer | Projected number of people in Service Delivery Division with the age of 0
1 | Integer | Projected number of people in Service Delivery Division with the age of 1
....
90+ | Integer | Projected number of people in Service Delivery Division that are 90 years old or greater
