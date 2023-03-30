![image showing sample visualization](https://user-images.githubusercontent.com/45638590/228588371-86b25a59-9c83-4897-8cc8-bb7695b3e4f9.png)

# ArcGIS Visualization
This tutorial will look at the steps necessary for ArcGIS Pro and ArcGIS Online as a geospatial data visualization tool.

----

## Setup Instructions
In preparation for this tutorial, you will need an organizational account with Esri. If you are a Brock user, you will sign into the software using your Brock credentials and the organization's URL brock.maps.arcgis.com.

**The Scenario**

We will be mapping tree sample data for the neighbourhood of Bridgewater near Niagara Falls and Chippewa. Tabular data was joined with the geospatial data creating a powerful connection that will allow us to visualize attributes such as diameter at breast height (DBH) and tree species. Although this example uses point data, the same general steps could apply to boundary files such as census tracts or municipal boundaries and associated tabular data.

----

## Visualization in ArcGIS Pro
Although there are many ways of creating visualizations using GIS technologies, we will explore some simple options for unique colours and proportional symbols. 

1. Run ArcGIS Pro and sign in using the organization's sign in workflow **insert link to video**
2. In a new map, add the joined layer from the previous exercise. Alternately, download the zipped shapefile [here](https://github.com/BrockDSL/ArcGIS_Visualization/blob/main/TreeSampleChippewa%20_XYTableToPoint.zip). Be sure to unzip the file before attempting these steps. **HINT: Right-click the zip file in Windows File Explorer and select *Extract all*. **

   ![image showing shapefile in arcgis pro window](https://user-images.githubusercontent.com/45638590/228621113-640a8714-8a22-42ae-807e-1ec3f1d70661.png)
  
3. From the Contents pane on the left side of the map view, double-click **map** ![image of map frame](https://user-images.githubusercontent.com/45638590/228622520-6ffda3b0-5324-47fa-9cc7-1fdf5aadeee4.png) to open the map frame properties. It is good practise to set the projection of the map frame to a local coordinate system.
4. From the map properties window, click **Coordinate System** and enter "UTM" in the search box.
5. Double-click **Projected Coordinate System".
6. Double-click **UTM** then **NAD 1983**.
7. Select **NAD 1983 UTM Zone 17N** for the Niagara area.
8. Click OK.

9. With the layer selected from the Contents listing, click the **Feature Layer** tab at the top.
10. Click **Symbology**. The Symbology pane appears to the right of the map view. 
11. From the **Primary Symbology** dropdown, select **Unique Values** and select Field1 -> Tree Species
12. Select a colour scheme from the dropdown.  
   ![image](https://user-images.githubusercontent.com/45638590/228628961-9c6ea78f-95d6-44aa-954e-e65f14c769d8.png)  
13. To vary symbology by size as well as colour, click ![image](https://user-images.githubusercontent.com/45638590/228629130-dea883ef-7aee-4a28-b44f-fadde23c7baf.png)
 from the Symbology pane.
14. Click **Size** and select **DBHTrunk** from the field dropdown.
15. Check the box to **Enable size range** and adjust the range to be 2 at minimum and 20 at maximum.
16. Scroll down and select **Show in Legend**. 

   ![image of symbology settings](https://user-images.githubusercontent.com/45638590/228630103-27c1eddb-6173-40a4-a737-ff3e4c8347c2.png)

The trees are now symbolized by colour for tree species and size for diameter at breast height (DBH).

   ![image showing symbolized trees](https://user-images.githubusercontent.com/45638590/228630488-88e7603f-9c2c-4e7c-9d78-617d76544d66.png)  

## Saving and Sharing

1. From the Contents listing, right-click the tree layer.
2. From the context menu, select **Sharing > Share as a layer package**. A layer package includes the assigned symbology and layer data your colleagues might need to work with the data effectively. 
3. Under **Start Packaging** choose **Save package to file** (alternately, you could upload the package to ArcGIS Online).
4. Under **Item Details** select a location and file name; summary and tags.
5. Under **Options** check the box to **Include Enterprise and UNC Path Data**. This option tells the software to include the data layers with the package. 

   ![image of Package Layers dialogue box](https://user-images.githubusercontent.com/45638590/228631866-0a00b8b7-2352-4ca3-916a-a767a0399d2f.png)

6. At the bottom of the the pane, click **Analyze** to see if there are any problems and then click **Package**. 
7. Open Windows File Explorer and navigate to the location where you saved the file ![image of a layer file](https://user-images.githubusercontent.com/45638590/228633466-1ea31a72-e04b-4d19-a9f5-67ea4d11dc54.png)  
This **.lpkx** can be shared with colleagues who are also using ArcGIS Pro.  

**NOTE: To use a .lpkx file, simply drag and drop the file to the map view from the Catalog pane.** 

## Visualization in ArcGIS Online

In some respects, visualization in ArcGIS Online offers more options and simpler workflows.

1. Go to https://arcgis.com and sign in to your ArcGIS Organization, brock.maps.arcgis.com > Brock university (when prompted with the Brock authentication page, enter your Brock credentials.
2. Click Map at the top of the screen. 
3. Click Add and change the folder from **My Content** to **ArcGIS Online**.
4. Enter the keywords "Chippewa tree tutorial" and click the plus sign to add the layer to your map.

   ![image of add layer in arcgis online](https://user-images.githubusercontent.com/45638590/228650762-ec325a71-09fc-43ba-b1ca-b7f921953ee8.png)

5. Click the back arrow to return to the layer listing ![image](https://user-images.githubusercontent.com/45638590/228650982-2a30be04-cb2c-435d-9f49-bc54cdaa3541.png)

6. Click the **Styles** button ![image](https://user-images.githubusercontent.com/45638590/228651117-f0f829ec-0889-4eae-a9dd-caa7a5838585.png) from the menu to the right.
7. In the Styles pane, make the following selections:
8. From Step One, click ![image add field button](https://user-images.githubusercontent.com/45638590/228651667-095d1d71-c2cc-42cc-a8d4-bab9cf88f7f0.png) then select the field to map, in this case, select **TreeSpecies**.
9. Click ![image add field button](https://user-images.githubusercontent.com/45638590/228651854-733cc3ba-65c1-48b0-a062-c5ef6092ff5a.png) again and select **DBHTrunk**. The symbols are updated with colours representing species and proportional symbols representing diameter. 
10. From Step 2 of the Styles pane, **Pick a Style**, select **Style Options** for types and size. There will be 2 options: one for unique symbols and one for counts and amounts.
11. Click style options for **unique symbols**. 

   ![image unique symbols options](https://user-images.githubusercontent.com/45638590/228652994-b177d8ee-5c6e-4c6f-9080-34444db42b9f.png)

13. Click the colour ramp for symbol style.  
14. For Outline Colour, select the black option. ![image colour option for outline](https://user-images.githubusercontent.com/45638590/228653257-4a9debd8-e25f-4fb2-a13c-852e84f4cb61.png)

15. Click Done then click the Counts and Amounts style options.  

   ![image](https://user-images.githubusercontent.com/45638590/228653512-667b6f1a-0037-43d8-a35c-113ffcd9dc19.png)

16. Scroll, if necessary, to change the size range from 90 to 20.  

   ![image](https://user-images.githubusercontent.com/45638590/228654737-4d6af67d-0edb-4314-bd6c-c03b798c556d.png)

17. Click Done twice.  
18. To give the map a little 'pop', click the effects options ![image](https://user-images.githubusercontent.com/45638590/228655102-85daf1b8-64e3-4f8a-940e-43f3f0f7e230.png) 
19. Toggle on the Drop Shadow option.  

   ![image of final map with trees symbolized](https://user-images.githubusercontent.com/45638590/228655289-a9109e1d-569a-4980-a071-a09d760c1140.png)  

20. Click the Save button from the left hand menu and save the map with a unique name.
21. To share your map as an image, click ![image print button](https://user-images.githubusercontent.com/45638590/228656138-a673d0c7-a606-4047-b569-07e43bbbe0a1.png)
22. Click Advanced Options and enter a title, set scale (~4500), author, copyright and check the box to include a legend.
23. Click Export. When the file is complete there will be a link to your file below the Export button.

   ![image](https://user-images.githubusercontent.com/45638590/228656813-240732c2-0813-4246-907d-4b8e22322731.png)  

   ![image of final map](https://user-images.githubusercontent.com/45638590/228657032-ca430898-220c-4584-82ba-4ac04928a95d.png)  

**NOTE: In some instances, the legend may be too large to fit on the page size map.**

"tree tutorial Chippewa data" tags to find the map on AGOL



----

## Next Steps (Optional)
Layout

----

**This tutorial is supported by the Brock University Research Lifecycle Department, Map, Data & GIS Library.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [maplib@brocku.ca](mailto:maplib@brocku.ca)**
