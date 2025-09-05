# Same web mapping application, Difference libraries

Whether you are adding a map to simply show locations on your web page or building a fully featured web mapping application for your spatial intelligence need, web mapping libraries are helpful places to start the development journey. In this five-part blog series, we will build the same web mapping applications using different popular libraries, then discussing key points related to building with that library.

## The goal
With this five-part blog series, we are hoping to achieve:

Showing implementation patterns of common workflows by creating the same app in popular mapping libraries.
- The libraries are: ArcGIS Maps SDK for JavaScript, Leaflet, MapLibre GL JS, and OpenLayers
- Determining and closing the gaps between libraries, so that developers can have smooth migrations.
- Illustrating the different implementation patterns for the libraries and their most suitable use cases
## What’s the app
The app shows common steps and typical workflows for web mapping applications in one app, including: loading data, visualizing data, displaying legends, popup window for more information, spatial querying, calculating statistics, and accessing location service.


The mapping application made with ArcGIS Maps SDK for JavaScript
In this application, we load and visualize census data and parks information in Hong Kong, then provides statistics on the number of parks, elderlies and kids within walking distance of a selected location. The number of elderlies and kids within walking distance is calculated by adding up the number of targeted demographics in census tracts that intersects with the walking area polygon.

Data is from Hong Kong’s Common Spatial Data Infrastructure (CSDI) portal, which is downloaded, then hosted for separately for data integrity and more convenient creation of different layer types or formats. Demographic data is from census in polygon and park (recreational grounds) data is a point layer in GeoJSON. Walking distance area is calculated with service area service in ArcGIS Location Service for consistency across the applications.


## This repo
This repo contains code for the apps in this project.
### ArcGIS Maps SDK for JavaScript
![arcgis-app](https://github.com/user-attachments/assets/47a13229-5143-411b-b474-6b039cd84fec)
