# Laura Cobham GEOM99 Technical Log 
(For start/end times, time spent, resources and next steps, see the Excel time log. This file is the outcomes)

Formatting: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## ArcGIS StoryMaps

2024/03/09

1. In StoryMaps I experimented with making custom themes to personalize your StoryMap. I made a theme called 'Sand' and customized the colours, font, basemap, and dividers so that the theme fit together.
2. For the rest of my time I played around with elements like timelines, image galleries, embedding external maps, and the different types of map tours. If we were to make a StoryMap, these are all functions that would be good and easy to use.

![sand](https://github.com/lacobham/geom99techlog/assets/146376068/26ef84de-988f-482b-8745-9ac79819b01d)

![waves](https://github.com/lacobham/geom99techlog/assets/146376068/8180a2d8-adbf-44f5-bf05-a32ced775458)

## ArcGIS Field Maps

2024/03/12

1. To experiment with the Field Maps mobile app I created a new point feature layer on AGOL and put that layer in a web map
1. 1. NOTE: I learned that you can create a point layer in the Field Maps Designer instead of in the AGOL item page, letting you customize other aspects too. You can also configure a form similar to Survey123 (can add different fields the user can fill with information).

![Fieldmaps](https://github.com/lacobham/geom99techlog/assets/146376068/7943e831-f96b-403e-a5db-3f770680353a)

2. I added a variety of points, some with photos and some without (most by moving the point from my actual location)
2. 1. NOTE: I learned that if you manually move the points most metadata will not autofill (e.g. elevation because the app can't guess the elevation at that point. Maybe try finding out if you can stop the user from doing this if that info is important?


## ArcGIS Dashboards

2024/03/12

1. To experiment with Dashboards I added a web map and chart, then added more widgets like indicators, gauges, embedding web pages, and rich text. I added the turtle icon from https://www.svgviewer.dev/s/364802/turtle.

![turtles](https://github.com/lacobham/geom99techlog/assets/146376068/25fabca7-0dd2-46b6-be58-9cdc8f68e7fa)

Link to dashboard: https://fleming.maps.arcgis.com/home/item.html?id=75773ea497444a1ab3d8e1cf5844b720

3. I then added red light camera data from the Toronto Open Data Portal and tried to make a more polished dashboard with different widgets.

![FinalDash](https://github.com/lacobham/geom99techlog/assets/146376068/1a0947b9-58f1-4953-bd67-4845525ae068)

Link to dashboard: https://www.arcgis.com/apps/dashboards/c0ae5db545df4a9fb953ef961a967d28

5. Overall, I think that so far the relevant widgets to our problem statement would be indicators, charts, and rich text. Gauges do not seem to be something relevant for our purposes.
   
## ArcGIS Experience Builder

2024/03/12

1. I experimented with Experience Builder by mostly recreating my previous Dashboard in a different environment. I tried out using charts, buttons, the basemap gallery, and images.

![ExpBuild](https://github.com/lacobham/geom99techlog/assets/146376068/1e37518b-5572-4b76-8c7c-6a8643c53575)

![FinalExpBuilder](https://github.com/lacobham/geom99techlog/assets/146376068/9f92e088-c9f1-47d2-90b6-93edbe5dbdd4)

1. I also read this link to try and understand the suitability modeler in Experience Builder to see if its something we could use in our collab project: https://doc.arcgis.com/en/web-appbuilder/latest/create-apps/widget-suitability-modeler.htm. I watched this video on the same topic: https://www.youtube.com/watch?v=Ha1H8LtkLX0.
1. Just from these sources it seems like its a super fast and easy way for someone to run a suitability analysis that may not be a GIS expert. You are able to change the weights and run the analysis over and over again, where it would take much longer in ArcGIS Pro. This likely would not be used for us to the analysis but could be something we look into for the client to quickly change criteria and rerun analysis on new areas.

Link to Experience: https://experience.arcgis.com/experience/56b1a5623dfe4962b8aec2c16a210200

~

Notes from Experience Builder tutorial (https://www.youtube.com/watch?v=zQMBhtQOwwY):

- Can insert URLs from Enterprise services

- Can insert multiple web maps at once

- Using dynamic attributes instead of manually changing each name/image is easier

- Triggers can make it zoom into specific features when clicked

Notes from video on making Experience Builder responsive (https://www.youtube.com/watch?v=lQcPleRqir0&list=PLGZUzt4E4O2L7N_0Wxkz8KLQhF-54kpFF&index=3):

- You can change between modes for different devices (mobile, tablet, desktop)

- The page will resize all the content to the device size and you can reconfigure (when you choose the 'custom' option, vs auto)

- Docked panels vs floating panels (similar to StoryMaps sidebar options)
