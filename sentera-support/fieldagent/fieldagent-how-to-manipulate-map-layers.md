---
description: >-
  Manipulating map layers in FieldAgent gives you the ability to see what's
  happening within a field by updating the colorization of a layer. This article
  pertains to how to do it with drone imagery.
---

# FieldAgent - How to Manipulate Map Layers

## FieldAgent Web <a href="#fieldagent_web" id="fieldagent_web"></a>

### Selecting a Map Layer <a href="#selecting_a_map_layer" id="selecting_a_map_layer"></a>

1\. [Navigate to the field](https://support.sentera.com/portal/en/kb/articles/navigating-to-a-field) where you would like to view a map layer.\
2\. Select the map layers icon <img src="https://support.sentera.com/galleryDocuments/edbsn5ac8e5b5bd243803adfd51f7f8ace6381acb419f2a9f13d80609ff135049d669f03a8f236e377e761b30456d1637528d?inline=true" alt="" data-size="line"> in the Map Layers section on the left.

![](https://support.sentera.com/galleryDocuments/edbsnc00884c0382dc840238c62145f0658937ba8f00256b2be19091ee00801468cb22ae3ffec3c04e76e817b9acee12be537?inline=true)\
\
3\. Locate and select the map layer you'd like to view.\
![](https://support.sentera.com/galleryDocuments/edbsn5ac8e5b5bd243803adfd51f7f8ace63822fb010d711bc470b55d73ba86e969e3684c7ae070cd2f69449f50929c5bc31c?inline=true)\
\
4\. Click on a selected map layer to view the map details page.\
\
This page provides options for editing how the map layer is displayed:\
![](https://support.sentera.com/galleryDocuments/edbsn661fdc951f68ab54566a17cd81457d53d93c8863fe8d95655834a7260c10c57135648b231bcfbfae15b7bbc20e501c46?inline=true)\
\
On the Map Details page, you'll see sections on the left for various ways to manipulate your map layer:

* Mosaic Details: Name/date of the survey. Click the pencil icon <img src="https://support.sentera.com/galleryDocuments/edbsn5ac8e5b5bd243803adfd51f7f8ace638be462fe2e53e294b2a083d44ff4dec9cd7ab2090ee0796184392bd361d94bcc6?inline=true" alt="" data-size="line"> to edit the name of the map layer.
* Mosaic Display Mode: Select "imagery" (standard map layer) or "zone map" (groups pixels to highlight trends). Note: RGB map layers do not have display mode options.
* Colorization: Change the values of how the histogram are displayed based on bins, max/min sliders, color scale, equal area, or equal spacing.&#x20;
  * Numbers of bins changes how many colors the values of the graph are divided into (the more colors, the more detail)
  * Max/min sliders change which pixels are included in the colorization (this can be used to highlight specific areas of a field)&#x20;
  * Color scale changes which colors are used in visualizing the map (our default is red to green, so the lowest values are in red and highest values are in green)&#x20;
  * Equal area gives each color the same number of pixels on the field (e.g., see best or worst areas of a simple map layer)
  * Equal spacing sets spacing by color and colors pixels as they fall into these intervals  (e.g., compare map layers from day-to-day or across different regions)&#x20;
* Clip to Field Boundary: Constrains the displayed image to the field boundary
* Opacity: Option to lower the opacity to see through the select map layer so you can compare multiple map layers at once&#x20;
* Download Files: Download the data in the format of your choice (available options are listed in the bottom left-hand column)&#x20;

## FieldAgent Desktop <a href="#fieldagent_desktop" id="fieldagent_desktop"></a>

When it comes to manipulating map layers, there are a few features in FieldAgent Desktop that are not available in FieldAgent Web. See below how to use this functionality in FieldAgent Desktop.&#x20;

1. Open Field View tab, then click Field Boundary, select the survey, and then select the Full Mosaic.
2. Select the NDVI/NDRE Toolbox from the field window.

<div align="left"><img src="https://support.sentera.com/galleryDocuments/edbsn061d40a1546bd7b42026d04c1ddb104960c8e8b402d2fa81a5e4e6d68c26cd42b21cced83ca6482074575f3a2f093d85?inline=true" alt="" width="375"></div>

3. Use the slide bars within the window similar to the functionality in FieldAgent Web, such as Color Map, Bins, Value, Equal Area.
4. To view statistics, select a shape file, then within the Statistics area, select average, minimum, and maximum values.\
   <img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:yellow;">**Note:**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">The statistics numbers may vary due to the numbers within the toolbox reflect the entire field, in the field reflect the statistics within the shape.</mark>

5\. To create a management zone, adjust the Zone Details and Gap Adjustments if necessary, then click the gear icon to generate zones.\
6\. To export the management zones as a shape file, click the Export icon. The file can then be imported into a farm management tool.

## Standard Examples for Manipulating Map Layers <a href="#standard_examples_for_manipulating_map_layers" id="standard_examples_for_manipulating_map_layers"></a>

### Highlight the Best Area <a href="#highlight_the_best_area" id="highlight_the_best_area"></a>

1. Bins: 1
2. Min/Max: Minimum slider moved to the right
3. Color Scale: Red to green

<div align="left"><figure><img src="../../.gitbook/assets/image (53).png" alt="" width="563"><figcaption></figcaption></figure></div>

Click show more under the slider to view the highlighted number of acres (or the best area in the field).

<div align="left"><figure><img src="../../.gitbook/assets/image (54).png" alt="" width="551"><figcaption></figcaption></figure></div>

### Highlight the Worst Area <a href="#highlight_the_worst_area" id="highlight_the_worst_area"></a>

* Bins: 1
* Min/Max: Maximum slider moved to the left.
* Color Scale: White to red

<div align="left"><figure><img src="../../.gitbook/assets/image (55).png" alt="" width="563"><figcaption></figcaption></figure></div>

### Highlight/Contrast the Best vs. Worst Areas <a href="#highlightcontrast_the_best_vs_worst_areas" id="highlightcontrast_the_best_vs_worst_areas"></a>

1. Display Mode: Zone Map
2. Bins: 2
3. Area Type: Equal Area
4. Color Scale: Red to green&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/image (56).png" alt="" width="563"><figcaption></figcaption></figure></div>

Need further assistance on this topic? Check out our video on YouTube:

{% embed url="https://www.youtube.com/watch?v=86iUHYFlsCU" %}
