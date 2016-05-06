[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/aliciatb/blight)
# Blight Prediction Project
The purpose of this project was to determine if any data features of a city can be used to predict blight for a given location.
## Data Source
These datasets were downloaded from the [course site](https://www.coursera.org/learn/datasci-capstone/supplement/D44tm/get-the-data), but are also available via [capstone project repo](https://github.com/uwescience/datasci_course_materials/tree/master/capstone/blight/data) on github. All of the data comes from [Socrata](https://www.socrata.com/) powered Detroit Data Portal, https://data.detroitmi.gov/.

## Data ETL
Before analysis of the data could be undertaken, all files were initially formatted using [Excel PowerQuery](https://support.office.com/en-us/article/Introduction-to-Microsoft-Power-Query-for-Excel-6E92E2F4-2079-4E1F-BAD5-89F6269CD605) for removal of line breaks and standardization of the street number and addresses. Then the data was loaded into [FME](https://www.safe.com/fme/fme-desktop/) to validate and standardize the geographic coordinates and output formatted incident and unique building files. Exploratory analysis and model creation was performed in [python notebooks](https://ipython.org/notebook.html) and [RStudio](https://www.rstudio.com/).
### FME Workflow Screenshot
![fme](https://github.com/aliciatb/blight/blob/master/fme_workflow.png)

## Data Analysis
* [Python Notebooks](http://mybinder.org/repo/aliciatb/blight)

## Predictions Models
* [RPubs]() *coming soon*
