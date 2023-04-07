## Background

This was a group project using the ETL method of data processing, Python Flask, JavaScript, HTML and Data Visualizations to create a tool for evaluating the relative air quality of California cities.


## Contributors: 

Shweta Joshi

Meera G K

Antonette Goroch

Dang Tran

Reed Zimpfer

## Introduction

In this Project we use publically available data to evaluate air pollution, which  is a leading cause of death across the globe, contributing to stroke, heart disease, lung cancer, and other respiratory illness. The goal of this project is to document and visualize the air quality of the California state area as a tool for promoting public health.

<img width="618" alt="image" src="https://user-images.githubusercontent.com/116701851/230517802-3e1f1db3-bd76-4c33-8087-cf52158a77da.png">


## Project Overview:

### Who is the target audience?
General Public

### Why is it relevant to them?
Health Awareness & Protection
Community Engagement & Advocacy
Planning & Decision Making

### About The Dataset
Our core dataset came from the Environmental Protection Agency (EPA)'s AQS (Air Quality System) database. 

https://www.epa.gov/air-trends/air-quality-cities-and-counties

The EPA is mandated by a number of laws, going back to its inception in the 1970s, to monitor and report key metrics about air quality annually. From this central database, we selected an initial file of Air Quality Statistics By City for the period 2000-2021.

This was the most recently available data and was published on May 4, 2022. It included 1600+ records and covered six of the most hazardous air pollutants covered by the Clean Air Act:
Ozone
Particulate Matter
Carbon Monoxide
Nitrogen Oxides
Sulfur Dioxide

## Data Processing and Software(ETL)

From the initial source data , a subset of data from the Sate California and Cities was extracted and converted into a CSV file. By applying the GeoApfy Key, basic lat/long coordinates were determined, then using the pandas dataframe, a final CSV data file was created.

Using the output CSV file, a Database was created using SQlite.

<img width="603" alt="image" src="https://user-images.githubusercontent.com/116701851/230516560-a68d1dd2-7181-4f0f-ade4-9a30b156140d.png">

## Flask & Dashboard
From the created Database, a python Flask was further deployed.

Then, using Javascript ,leaflet and HTML, a dashboard was created in the local port. The dashboard includes a statewide map showing the pollutant level for each California city, and whether or not it is above/below the established healthy level via a pop up hover box.

<img width="1276" alt="image" src="https://user-images.githubusercontent.com/116701851/230517026-5eca9799-96a7-4cec-af9a-2449e140c696.png">

The dashboard also includes Bar and Linear graphs that plot the Annual mean of NO2 and PM2.5 on each City and Year.

<img width="596" alt="image" src="https://user-images.githubusercontent.com/116701851/230517490-cdcfa1c8-b3d3-41ca-b0a5-e0af6bc9ea64.png">

<img width="595" alt="image" src="https://user-images.githubusercontent.com/116701851/230517465-264a2f96-fe29-403f-9d51-968a895a7079.png">

<img width="624" alt="image" src="https://user-images.githubusercontent.com/116701851/230517527-df7e89ca-ea09-4f9c-808a-8950412dfe0a.png">

<img width="610" alt="image" src="https://user-images.githubusercontent.com/116701851/230517559-6116ded2-6068-4d28-8d99-fe0306b38d0b.png">

## Data Visualization and Analysis

Our analysis showed that pollutant Levels of CO, SO2, and PM10 have been continuously dropping since the EPA began monitoring, suggesting moderate to good air conditions in the State overall. Still, we see that Ozone, NO2, and PM2.5 haven't dropped that much are likely related to the large number of factories, large number of vehicles, and other source of pollution that are still not under well controlled.


## Conclusions

Though CA air quality has been improved in recent years, there are still pollutants (Ozone, NO2, and PM2.5) that retain a high pollution Level. 
Effort should continuously be made to reduce them. and tools such as this can help facilitate that. How can we make a difference? Drive less, use less electricity, don't burn wood or trash, support measures in your community that can cut air pollution, etc.
Also air quality continues to worsen in cities across the world, especially in low-income countries and developing countries.  Cooperation should be setup among countries in combating air pollution. Again, tools like this one can help facilitate this process.





