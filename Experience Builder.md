# Laura Cobham GEOM99 Technical Log 
(For start/end times, time spent, resources and next steps, see the Excel time log. This file is the outcomes)

Formatting: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## ArcGIS Experience Builder (Suitability Modeler)

2024/03/19

1. I used layers from GEOM109 to attempt a suitability analysis using suitability modeler in Experience Builder. To get the raster layers into AGOL I used the manage tile cache, export tile cache, and share package tools. I used this video as a reference: https://www.youtube.com/watch?v=bQmOpcJrf0c
2. I put all 5 layers (landcover/wolf density/slope/road distance/campsites and trail distance) into a web map hoping that this would then connect to the suitability modeler widget in Experience Builder.
![Capture](https://github.com/lacobham/geom99techlog/assets/146376068/1e825720-d9dc-422c-9118-a65d9c493a18)

1.I then realized that this is not the way that the layers go into the suitability modeler, but instead they have to be published on ArcGIS Server as an image service based on the documentation that I looked into:
https://pro.arcgis.com/en/pro-app/3.1/help/sharing/overview/publish-an-image-service.htm
https://doc.arcgis.com/en/geoplanner/latest/documentation/publish-your-data-as-a-weighted-overlay-service-portal-.htm
2. ![Capture 2](https://github.com/lacobham/geom99techlog/assets/146376068/17110ec4-f4ff-4b7d-91d1-5a3a155afd5e)

This seems like it is outside the scope of the project/problem statement and would be something to deal with in our collab if needed, but for now I decided to focus on other more relevant aspects of the project.
