# Kindley_ENV872_Project

Repository for Sierra Kindley's Environmental Data Analytics final project at Duke University (spring 2020).

## Summary

This repository was created for Sierra Kindley's Environmental Data Analytics final project at Duke University (spring 2020). 

The five Soil Climate Analysis Network (SCAN) datasets included in this repository contain daily soil moisture and climate data at sites located in the state of California. Each dataset contains data from a single sampling site in California, so a total of five sites are represented. These sites are located at different elevations and in various regions of the state.

The primary aim of this project is to analyze the daily soil moisture and climate data from the selected sites in California and identify trends in soil moisture and soil temperature relative to soil depth, solar radiation, site (specifically with regards to elevation--all sites are located at different elevations), and time of year. These analyses will be performed on data from 2015 to 2019 (01/01/2015 to 12/31/2019).

## Investigators

Sierra Kindley - Nicholas School of the Environment, Duke University (sierra.kindley@duke.edu)

## Keywords

soil, soil temperature, soil moisture, California, climate, agriculture

## Database Information

Data were collected using the Soil Climate Analysis Network (SCAN) (https://wcc.sc.egov.usda.gov/nwcc/rgrpt?report=daily_scan_por). SCAN is a comprehensive, nationwide soil moisture and climate information system designed to provide data to support natural resource assessments and conservation activities. Administered by the United States Department of Agriculture Natural Resources Conservation Service (NRCS) through the National Water and Climate Center (NWCC), in cooperation with the NRCS National Soil Survey Center, the system focuses on agricultural areas of the U.S. monitoring soil temperature and soil moisture content at several depths, soil water level, air temperature, relative humidity, solar radiation, wind, precipitation, barometric pressure, and more. 
The following selections were made within the dataset:
* California (Geographic Area)
* Bodie Hills, Cochora Ranch, Deep Springs, Ford Dry Lake, French Gulch (Site Selection)
* Daily SCAN Standard Report - Period of Record (Data Report Type)
* Download CSV (spreadsheet)

The CSV files were saved as 'SCAN_BodieHillsCA_raw.csv', 'SCAN_CochoraRanchCA_raw.csv', 'SCAN_DeepSpringsCA_raw.csv', 'SCAN_FordDryLakeCA_raw.csv', and 'SCAN_FrenchGulchCA_raw.csv'.

Data were first accessed on 2020-04-10.

## Folder structure, file formats, and naming conventions 

Within this repository are the following folders: Code, Data, and Output. The 'Code' folder contains R scripts and Rmd files pertaining to the project. The 'Data' folder contains two folders ('Raw' and 'Processed')--one containing raw data (primarily .csv files) and one for processed data (primarily .csv files). The 'Output' folder contains any outputs (e.g. figures, graphs) generated from data analysis and visualization (primarily .png files).

Data files are named according to the following naming convention: 'databasename_location_stage.format', where:

**databasename** refers to the database from which the data originated

**location** refers to the site in the state of California at which the data was collected

**stage** refers to the stage in the data management pipeline (e.g. raw, cleaned, processed)

**format** is a non-proprietary file format (e.g., .csv, .txt)

## Metadata

Each dataset in the repository contains the following data columns:

Date: Month/Day/Year
Station Id: Station ID number
Air Temperature Maximum: Maximum air temperature - sub-hourly sampling frequency (degrees Fahrenheit)
Air Temperature Minimum: Minimum air temperature - sub-hourly sampling frequency (degrees Fahrenheit)
Precipitation Increment: Total precipitation (inches)
Relative Humidity: Relative humidity (%)
Wind Speed Maximum: Maximum wind speed (miles/hour)
Wind Speed Average: Average wind speed (miles/hour)
Solar Radiation Average: Average solar radiation (watts/meter squared)
Solar Radiation/langley Total: Total solar radiation (Langleys)
Vapor Pressure - Partial: Partial vapor pressure (inches Hg)
Vapor Pressure - Saturated: Saturated vapor pressure (inches Hg)
Soil Moisture Percent -2in: Percent volumetric soil moisture at 2 inches depth (%)
Soil Moisture Percent -4in: Percent volumetric soil moisture at 4 inches depth (%)
Soil Moisture Percent -8in: Percent volumetric soil moisture at 8 inches depth (%)
Soil Moisture Percent -20in: Percent volumetric soil moisture at 20 inches depth (%)
Soil Moisture Percent -40in: Percent volumetric soil moisture at 40 inches depth (%)  
Soil Temperature Observed -2in: Observed soil temperature at 2 inches depth (degrees Fahrenheit)
Soil Temperature Observed -4in: Observed soil temperature at 4 inches depth (degrees Fahrenheit)
Soil Temperature Observed -8in: Observed soil temperature at 8 inches depth (degrees Fahrenheit)
Soil Temperature Observed -20in: Observed soil temperature at 20 inches depth (degrees Fahrenheit)
Soil Temperature Observed -40in: Observed soil temperature at 40 inches depth (degrees Fahrenheit)

## Quality assurance/quality control

Each dataset in the repository includes the following quality control flags:

V: valid - validated data
N: no profile - no profile for automated validation
E: edit - minor adjustment for sensor noise
B: back estimate - regression-based estimate for homogenizing collocated Snow Course and Snow Pillow data sets
K: estimate
X: external estimate
S: suspect - suspect data


Each dataset in the repository includes the following quality assurance flags:

U: unknown
R: raw - no human review
P: provisional - preliminary human review
A: approved - processing and final review completed
