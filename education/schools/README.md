# List of Schools

## Description
The Transportation Services Division of the City of Toronto compiled [this dataset](csv/school_master.csv) `school_master.csv` for the Vision Zero Challenge, using multiple sources described below. 

This dataset contains the master list of all 1327 schools located in Toronto. The list spans the 4 school boards, private schools, and post-secondary institutions. The schools on this list span 4 levels: Elementary, Secondary, Adult High Schools, and Post-Secondary schools. Middle schools are classified as elementary schools.

The Ontario Private Schools Database contains all private schools in the province, and was last updated in 2018.

The Online TDSB and TCDSB includes all currently operating TDSB and TCDSB schools, updated in 2017.

The Toronto Police Service Database of schools contains most schools in Toronto, including all post-secondary institutions, and the majority of private schools, updated in  2014. The data has been adjusted for schools that have opened and closed since 2014. 

**Format:** Comma Seperated Values (CSV)

## Relevance to the Vision Zero Challenge
School children are one of the six emphasis areas defined under the City of Toronto's Vision Zero Road Safety Plan, and are the focus of a number of existing and planned safety measures. 

## Data Dictionary
| Column Name | Type | Description |
|-------------|------|-------------|
| ID | Integer | Unique identifier | 
| Name | Text | Name of institution | 
SCL_LVL | Text| Level of schooling (elementary, secondary, or adult) if its not a post-secondary institution
SCL_TP | Text| Abbreviation of the type of school board
BRD_NAME| Text| Full name of the school board
SCL_TP_DSC|Text|Type of school board
ADD_FULL|Text|Address of the school
POSTAL_CD|Text|Postal Code
MUN|Text|Former municipality the school is located in. East York is included in Toronto, which is also referred to as former Toronto
LATITUDE|Float|Coordinates of the school
LONGITUDE|Float|Coordinates of the school
