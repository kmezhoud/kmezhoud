---
title: "Biodiversity Map Tracking using Open Biodiversity Datasets"
external_link: https://kmezhoud.shinyapps.io/biodiversity/
date: '2022-02-12T00:00:00Z'
summary: Biodiversity
tags:
- r
- Shiny
image:
  caption: screenshot
  focal_point: Smart
url_code: https://kmezhoud.github.io/learn_by_example/biodiversity_performance/biodiversity_performance.html
url_pdf: ''
url_slides: ''
url_video: ''
---

+ biodiversity is a complete R package
  + Build/Check/Test package
+ Docker container is available.
+ Extend search to multiple countries: Poland, Switzerland, Germany, France, Spain.
+ Convert csv files to sqlite database.
  + Faster read of tables
  + focus search on selcted tables
+ Add popup to select interested countries to focus on. 
  + Reduce waiting time and improve reactivity of the App.
  + Limit functionalities to wanted countries
+ Add Progressbar to inform the user what the app is doing
+ Starting Map position focus of the mean(s) of latitude(s) and longitude(s) of selected Countri(es).
  + User do not need to scroll the map to selected countries.
+ Add a Layout control panel for existing Kingdom
  + Rapid Overview of the position of Animals, Plants and Others
  + User can focus search by Kingdom
+ User can search by `vernacularName`, the app returns `scientificName` and vice versa.
+ After searching and selected species from the search engine, the Map  go and Focus on item position with:
  + Indicate the position with red circle, and
  + Open popup with all needed information: 
    + External link to original data,
    + How many times the species has been encountered,
    + Individual Count in each encounter,
    + Image,
    + Link to reference.
+ Button to iterate search if user want to change/select other countries
+ Info Boxes indicating the total of each existing king.
+ CSS styling with logos in header, Absolute Panel with transparent Button