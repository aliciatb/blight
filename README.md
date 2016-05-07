[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/aliciatb/blight)
# Blight Prediction Project
The purpose of this project was to determine if any data features of a city can be used to predict blight for a given location.
## Data Source
These datasets were downloaded from the [course site](https://www.coursera.org/learn/datasci-capstone/supplement/D44tm/get-the-data), but are also available via [capstone project repo](https://github.com/uwescience/datasci_course_materials/tree/master/capstone/blight/data) on github. All of the data comes from [Socrata](https://www.socrata.com/) powered Detroit Data Portal, https://data.detroitmi.gov/.

## Data ETL & Preprocessing
Before analysis of the data could be undertaken, all files were initially formatted using [Excel PowerQuery](https://support.office.com/en-us/article/Introduction-to-Microsoft-Power-Query-for-Excel-6E92E2F4-2079-4E1F-BAD5-89F6269CD605) for removal of line breaks and standardization of the street number and addresses. Then the data was loaded into [FME](https://www.safe.com/fme/fme-desktop/) to validate and standardize the geographic coordinates and create well formatted incident and unique building files. Features were generated within FME workflow of total 311 calls, crimes and blight violations for a building. A [Property Values dataset](https://data.detroitmi.gov/d/ug2h-q3n5) found on the [Detroit Data Portal](https://data.detroitmi.gov/) that included appraised and taxed values, sales price, tax status, and whether it had been improved at any point was also joined to the data so those features could be included in the models and also served to limit dataset so that building lacking predictive features were filtered from final data. 

### FME Workflow Screenshot
![fme](https://github.com/aliciatb/blight/blob/master/fme_workflow.png)

## Exploratory Data Analysis
* [Python Notebooks](http://mybinder.org/repo/aliciatb/blight)

## Predictions Models
* [RPubs]() *coming soon*
