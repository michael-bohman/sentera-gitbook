---
description: >-
  Shapes/zones can be created on a field level to call out specific areas of
  interest. These areas can then be compared quantitatively.
---

# FieldAgent - Creating Zones and Comparing Areas of a Field

## Comparing Satellite Zones In FieldAgent Web <a href="#comparing_satellite_zones_in_fieldagent_web" id="comparing_satellite_zones_in_fieldagent_web"></a>

Satellite Imagery is useful for monitoring your fields from any location. Use satellite to check-in routinely or as a first response after receiving a FieldAgent Notifications. Satellite images may be able to detect and diagnose the conditions in your field. If you're still curious about what's happening in your field, you can use satellite images to pinpoint areas for drone or ground scouting.

### Quantitative (Number Based) Comparisons

Visual comparisons can work well and may help with most decision making, however values allow you to put numbers to areas and compare without bias.

Let's say we are comparing three seed varieties or three farming practices in three different locations within a field. We can start by looking at an NDVI crop health satellite layer and performing a visual comparison. In the example below, we can see that all three sections of the field seem to be performing relatively well. If we had to say, the middle section appears to be performing the “worst”, although still very green.

<figure><img src="../../.gitbook/assets/1 (3).png" alt=""><figcaption></figcaption></figure>

Each pixel in an NDVI or NDRE health map contains a health value for that location. We’ll get into more on these values in the next section, but for now, understand that the higher the number, the “healthier” the location is.

To view average values for each location in this field:

1. Add new zones to the field by clicking on the + button in the zones section.

<div align="left"><figure><img src="../../.gitbook/assets/2 (3).png" alt=""><figcaption></figcaption></figure></div>

2. Use the toolbar on the right to create a zone
   1. Add Polygons: Select one of the drawing tools <img src="../../.gitbook/assets/image (314).png" alt="" data-size="line"> <img src="../../.gitbook/assets/image (313).png" alt="" data-size="line"> <img src="../../.gitbook/assets/image (316).png" alt="" data-size="line"> When you are done, select Finish where you selected the drawing tool.
   2. Move Corners: Select the corner edit tool <img src="https://support.sentera.com/galleryDocuments/edbsn4c492f3582175afca62e4c09172825e024abc1f3b641d1783b4af2eb28cf969e43a91be63c64538911003abf010a4b58?inline=true" alt="" data-size="line">on the right to move corners. When you are done, select Finish where you selected the edit corner tool.
   3. Move Shape: Select the drag layers tool ![](https://support.sentera.com/galleryDocuments/edbsn228b010627544193d89d5d507d23ee476d56caf045877dd60389460512939da6aa1edb64db1bfef67181cbcab0bc1588?inline=true) then click and drag the zone to move its locations. When you are done, select Finish where you selected the drag layers tool.
   4. Delete a Boundary: Select the erase tool ![](https://support.sentera.com/galleryDocuments/edbsn228b010627544193d89d5d507d23ee47f94624d1cfc7c12b44123222ae86381b1a83c99b7f46441d58b6f6e06e61e4b3?inline=true) and then any polygons you’d like to delete. When you are done, select Finish where you selected the erase tool.
3. Name the zone, click Finish on the right side of the window to complete your drawing and then click Save.
4. Repeat this for each zone you’d like to compare
5. Then add an NDVI or NDRE map layer to your screen.
6. Click on a layer to view the details of that layer.
7. Scroll to the bottom of the screen on the left and look for the section labeled Zone Statistics. Here you’ll find the average NDVI or NDRE value for each zone you’ve created as well as an average for the full field boundary.

<div align="left"><figure><img src="../../.gitbook/assets/5.png" alt=""><figcaption></figcaption></figure></div>

8. Click Download Shapefile under the display mode section.\
   ![](https://support.sentera.com/galleryDocuments/edbsn0d85107ab9c33a5924e5e3db62aaf12a7bd9ce661ad69d7b6943054dc81df4845a55e6cb697b5589389987ed42f18779?inline=true)\
   The downloaded file can now be used in a tool such as SMS to create a prescription.

{% embed url="https://demo.arcade.software/0jfgI7gC8s6KQtDEoa6P?embed=" %}

This is useful when comparing zones within a field as shown in the above example, but can also be useful when comparing two fields. Simply compare the Field Boundary Zone Statistics of a Satellite layer on one field to that of another field. This tool can also be useful for evaluating drydown progression. Below are 5 dates with their NDVI map layers, as well as the Field Boundary NDVI value. You can see the progression from a lush field, to one that is dried down and ready for harvest. By comparing the values across fields, or within zones of a single field, you may be able to direct harvest order.

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><p><img src="https://support.sentera.com/galleryDocuments/edbsn90c06e45df05e962cb68ab831f615dcc2bc50f177c713c283c515253588c82a56ba7d2f2858a1227543baa13f9e3dcc7?inline=true" alt="" data-size="original"><br></p><p>August 22nd<br></p></td><td valign="top"><p><img src="https://support.sentera.com/galleryDocuments/edbsn59bc93adbb84bf135987ff24c3cd899af74bb1a07e3a9df341b415bd1646994aa107a80c8d75d3190c087871e097572a?inline=true" alt=""><br></p><p>September 6th<br></p></td><td valign="top"><p><img src="https://support.sentera.com/galleryDocuments/edbsn59bc93adbb84bf135987ff24c3cd899a2754fc1855323755d6d1a01477f961680ff546e626e88aad3143348d76ebc6ae?inline=true" alt=""><br></p><p>September 16th<br></p></td><td valign="top"><p><img src="https://support.sentera.com/galleryDocuments/edbsn1fc6f2b19d8dc3c971cb249de300d6e73f8f02f47525bfeff585ee6c406aa62514885f1ce854bc750ec0555eb01af3b5?inline=true" alt=""><br></p><p>September 21st<br></p></td><td valign="top"><p><img src="https://support.sentera.com/galleryDocuments/edbsn59bc93adbb84bf135987ff24c3cd899aa280825818b5902e6e8a7c67fbe897dd40e00b160ed0a49fb3d996d5ae3cade7?inline=true" alt=""><br></p><p>September 26th<br></p></td></tr><tr><td valign="top">NDVI Value: 0.84<br></td><td valign="top">NDVI Value: 0.74<br></td><td valign="top">NDVI Value: 0.34<br></td><td valign="top">NDVI Value: 0.29<br></td><td valign="top">NDVI Value: 0.19<br></td></tr></tbody></table>

### Exporting your satellite zone maps&#x20;

to learn more about exporting your zone maps click [HERE](create-and-export-management-zones-and-prescription-files.md)

## Comparing Stand/Tassel of Areas in FieldAgent Web <a href="#comparing_standtassel_of_areas_in_fieldagent_web" id="comparing_standtassel_of_areas_in_fieldagent_web"></a>

1. Ensure each area you'd like to compare has a zone. If necessary create a zone by pressing the + button under the Zones section on a field page. Learn how to create a Zone [HERE](fieldagent-create-edit-and-delete-a-field-boundary.md).
2. Turn on a Stand Count Layer with the discs and numbers.

<div align="left"><figure><img src="../../.gitbook/assets/image (317).png" alt="" width="563"><figcaption></figcaption></figure></div>

3. Click on the individual layer to open the layer details.

<div align="left"><figure><img src="../../.gitbook/assets/image (318).png" alt=""><figcaption></figcaption></figure></div>

4. Under the Zone Statistics section, you'll see your list of zones, as well as their Minimum, Maximum, and Average Stand or Tassel Counts.

<div align="left"><figure><img src="../../.gitbook/assets/image (319).png" alt="" width="339"><figcaption></figcaption></figure></div>

## Example Stand Count Comparison <a href="#example_stand_count_comparison" id="example_stand_count_comparison"></a>

The values of two zones can be compared.\
In this example we are comparing the right and left halves of a field, each planted with a different seed variety.\
By visually altering the colorizations, setting the Bins to 2, we can see that the Right half of the field should have a lower average stand count.\
![](https://support.sentera.com/galleryDocuments/edbsnd68c8eb2ac09a4361648bdf7d3ce3df43fd020e51567f039789a9d671efd21dc493f91a519dbb856e6a1e755df5d4711?inline=true)\
\
Using the zone statistics, we can see the seed variety on the right has an average of \~2k more plants per acre.

<div align="left"><figure><img src="../../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure></div>

<div align="left"><figure><img src="../../.gitbook/assets/image (321).png" alt=""><figcaption></figcaption></figure></div>

### Exporting your Stand/Tassel zone maps  <a href="#exporting_your_standtassel_zone_maps" id="exporting_your_standtassel_zone_maps"></a>

to learn more about exporting your zone maps click [HERE](create-and-export-management-zones-and-prescription-files.md)

### Comparing NDVI/NDRE of Areas in FieldAgent Desktop <a href="#comparing_ndvindre_of_areas_in_fieldagent_desktop" id="comparing_ndvindre_of_areas_in_fieldagent_desktop"></a>

1. Locate and turn on the NDVI or NDRE survey you'd like to perform a comparison with.\
   ![](https://support.sentera.com/galleryDocuments/edbsn33fb58acb83f84ab0f8a4eb19a0acf12ae645e83ea57142f14c1a52780c2d691c201d766af254f8db2cce5a264f213d0?inline=true)\

2. Turn on all shapes you'd like to compare the area of. If you need to create a shape, click Add or learn how to create shapes on FieldAgent Desktop [HERE](https://support.sentera.com/portal/en/kb/articles/fieldagent-drawing-fields#Add_a_Call_Out_Area_in_the_Field_with_a_Shape_File).\
   ![](https://support.sentera.com/galleryDocuments/edbsn40c9e0766013e33938ed9b0e7312eef8172b701de2ceb52c66bf707a1a03e285ea9cf7e361e43a5c05250746f78b47b4?inline=true)
3. Open the Toolbox.\
   ![](https://support.sentera.com/galleryDocuments/edbsn33fb58acb83f84ab0f8a4eb19a0acf122350cc49a7a8b1519ffe88685ac59a4e699a4728efc83df78b66073b236157d8?inline=true)
4. Select the Avg checkbox in the lower right. The number in the toolbox is the average for the whole field boundary.\
   ![](https://support.sentera.com/galleryDocuments/edbsn65f8467d5662ee436e9c25806bca576624bbdfa4bdac303b20204c2e15b357c80c665c32008eaed572a6453c5f6f29c0?inline=true)
5. You'll see the Average NDVI or NDRE values display as part of each selected shape.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/two zones for art.jpg" alt="" width="563"><figcaption></figcaption></figure></div>

6. If a report is generated at this point, it will include
   * The map image you selected.
   * The average values for each selected shape displayed on the map.
   * The average value for the whole field boundary.
   * The acreage of each shape.
   * The acreage of each color range in the whole field boundary.
   * Any notes that you add to describe your field.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/report for art 3.2.jpg" alt="" width="563"><figcaption></figcaption></figure></div>
