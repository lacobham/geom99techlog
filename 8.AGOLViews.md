# Laura Cobham GEOM99 Technical Log 
(For start/end times, time spent, resources and next steps, see the Excel time log. This file is the outcomes)

Formatting: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## ArcGIS Online Layer Views

2024/03/28

- First I created a new Survey in Survey123 that had a field I would want to hide (email address). This also created a new feature layer, since there was a question in it asking the user to enter where they spotted a turtle.

![view1](https://github.com/lacobham/geom99techlog/assets/146376068/c6ad9683-daa5-4bdd-aecf-547e6436539e)

- I excluded irrelevant or confidential fields (email address, creator, creation date, editor, edit date)

![View2](https://github.com/lacobham/geom99techlog/assets/146376068/ea4b49b4-883d-4f51-a853-b7fcaf642508)

- I also drew a polygon around Ontario to limit the points to a smaller study area.

![View 3](https://github.com/lacobham/geom99techlog/assets/146376068/5e9a2f2d-d442-47f0-bb9f-41425a145d85)

![View4](https://github.com/lacobham/geom99techlog/assets/146376068/ad42cb26-cd5d-4180-aa2f-9c135c457aaf)

- I tested the view by adding 2 points to the survey, one in Ontario and one in the US. This meant that when only the view layer was turned on only one point showed up (the one in Ontario), and with the original feature layer on both points would show.

![ViewmapOnt](https://github.com/lacobham/geom99techlog/assets/146376068/fa9d66e3-b382-4dba-bb59-273bee2dcbdb)

![Viewmapboth](https://github.com/lacobham/geom99techlog/assets/146376068/1faa4330-e3a7-44e8-ad2a-58c3ceb00f64)

- Something I learned was that the view creates a new hosted feature layer. I originally assumed that a view was just an add-on to the original feature layer, but it is its own layer that is also a view. I also assumed that limiting the study area would prompt the user in the survey to enter a point inside the study area, but I learned that the purpose of views is more to filter the data to relevant points rather than change the user input.

- I visited this link in the documentation as a guide: https://doc.arcgis.com/en/arcgis-online/manage-data/create-hosted-views.htm
- After these steps I also watched Shawn's video on views to learn more: https://www.youtube.com/watch?v=AM7zoGQ4XxY 

The map can be found here: https://fleming.maps.arcgis.com/apps/mapviewer/index.html?webmap=c74c4aaa6cb945d6a958247ff7376afc
The survey can be found here: https://fleming.maps.arcgis.com/home/item.html?id=6a0bdc28030f4593ad442327066c2738
