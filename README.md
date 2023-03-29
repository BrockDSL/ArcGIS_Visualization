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
.
14. Click **Size** and select **DBHTrunk** from the field dropdown.
15. Check the box to **Enable size range** and adjust the range to be 2 at minimum and 20 at maximum.
16. Scroll down and select **Show in Legend**. 

![image of symbology settings](https://user-images.githubusercontent.com/45638590/228629406-7c4b5bf5-e7e7-40f6-98a4-4177f3246ada.png)

display tree species by colour
group items
add attribute > size > DBH

![image](https://user-images.githubusercontent.com/45638590/228626221-07574b43-fa20-4c28-8b13-c9b116a378fc.png)

adjust settings

save




----

## Next Steps (Optional)
This is where you can add any additional resources, follow up tutorial, or workshop reccomendations that users might use to continue learning about the tool described in the tutorial.  The more the better!

----

**End notes**
This is where you mention the DSL, MDGL, or Research Lifecycle department and put in contact information.  An example of what this might look like is:

**This tutorial is supported by the Brock University Research Lifecycle Department.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [DSL@Brocku.ca](mailto:DSL@Brocku.ca)**
