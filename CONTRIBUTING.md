# How to Contribute to this Repository

When working on a dataset, convert the dataset card to an Issue in the [repository's Project](https://github.com/CityofToronto/bdit_vz_challenge/projects/1), assign yourself to the issue, and create a new branch for that dataset. Each dataset should have its own subfolder under the broad categories of data (Entertainment, Childcare, Transportation Infrastructure), and the description for that dataset should be in a `readme.md` file in that folder. Once you have finished writing up the ReadMe, commit your changes (while tagging the issue), sync them with Github, and open a Pull Request for that contribution. Someone else on the team will review your changes and suggest corrections or accept and merge.

## What the README Should Contain

### Description

High-level overview of what the data is, where it comes from, what it's about. Link to the OpenData page if it's already available on OpenData.

### Why It's Relevant

How does the dataset relate to Vision Zero and the 3 emphasis demographics of the Challenge: seniors, newcomers and school children? 

### Data Dictionary

Create a markdown table like the following, include each column, its type, and a description of the field.

| Column Name | Type | Description |
|-------------|------|-------------|
| Primary key  | Integer | Uniquely identifies each row | 
| Name of thingy | Text | Names the thing | 

### Limitations

Detail any caveats and limitations for the dataset. E.g.:
 - sidewalk data is a couple years old; or
 - can't guarantee accuracy of count data.
