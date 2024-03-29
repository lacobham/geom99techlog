# Laura Cobham GEOM99 Technical Log 
(For start/end times, time spent, resources and next steps, see the Excel time log. This file is the outcomes)

Formatting: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## Linking Survey123 and Dashboards

2024/03/20

1. Previously, I thought that only ArcGIS Field Maps would live update data onto Dashboards, but after our group check-in we learned that Survey123 will do it as well. So I created a new survey for a user to input point data to test on Dashboards.

Link to survery: https://survey123.arcgis.com/share/8b79a8a926144c98b859ec6b42cc25f9?portalUrl=https://Fleming.maps.arcgis.com

![image](https://github.com/lacobham/geom99techlog/assets/146376068/84e5adf7-9f9e-4a05-b1e2-c3d97ee5fc94)

![image](https://github.com/lacobham/geom99techlog/assets/146376068/2ad07797-7881-404a-ae34-6988549e1355)

2. The map in the survey created a new point feature layer which I then put in a web map, and then into a dashboard.

Link to dashboard: https://fleming.maps.arcgis.com/apps/dashboards/fa63ba0c4aa14cdfa19b0bf84f4b4c97#mode=edit

![image](https://github.com/lacobham/geom99techlog/assets/146376068/ffeb39ae-f84e-4128-b09b-736c2bfec754)

3. In this dashboard, I learned that you can embed the survey so anyone can fill out the form and refresh the page to see the map update or to fill it out again. The charts and indicator also update. Also, that if someone logs that they saw multiple turtles at one time, you need to make sure you select 'sum' instead of 'count' so that it won't simply count the amount of people who filled out the survey.
4. I also learned that you can use an SVG as the symbol on a web map, so instead of having a legend for the map the indicator basically serves as one.
