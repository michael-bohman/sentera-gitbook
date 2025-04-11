# Create and Export Management Zones and Prescription Files

<img src="https://img.zohostatic.com/zde/static/images/lights.png" alt="" data-size="line"> <mark style="background-color:green;">**Now available for satellite imagery!**</mark>

Management zones are used to group the data of a detailed health map into simple shapes that can then be exported as a prescription file. Below is an example of a zone map (left) and the health map which was used to create the management zone.\
​\
![](https://support.sentera.com/galleryDocuments/edbsne2eac7942aba0a0a63eb4ef8c805d33f9535eaebdfcd61b4ba7916e9f65d21e98a0684f32be86ab713ee5bb33db4c544?inline=true)![](https://support.sentera.com/galleryDocuments/edbsn4c492f3582175afca62e4c09172825e0c52c23cc01604dbea309f4a67ff82ea9850de0ee5c947bff820d1fb07224c914?inline=true)

### Management Zones on Web <a href="#managment_zones_on_web" id="managment_zones_on_web"></a>

1. Open [FieldAgent.Sentera.com](http://fieldagent.sentera.com/) and [navigate to the field](https://support.sentera.com/portal/en/kb/articles/navigating-to-a-field) you'd like to create a zone map for.
2. Open the map layer you'd like to create the zone map from. Note: RGB layers cannot be turned into zone maps.&#x20;

&#x20;Some types of map layers that can be turned into zone maps include:

* NDVI or NDRE Satellite Imagery
* NDVI or NDRE QuickTiles or Mosaics
* Populations Maps (from a Stand Count)
* Tassel Maps (from a Tassel Count)

3. Set the mosaic display mode to Zone map\
   ![](https://support.sentera.com/galleryDocuments/edbsn57b2ae062375c2347df5604f3e154e948fa0adca3ee672ade4348df901919e3145c356a5c031b4d049ee17c9173f1f1c?inline=true)
4. [Manipulate the layer](https://support.sentera.com/portal/en/kb/articles/manipulate-map-layers) as you'd like:
   * Select the number of bins (colors)
   * Set the minimum and maximum values to be included
5. Click Download Shapefile\
   ![](https://support.sentera.com/galleryDocuments/edbsn0d85107ab9c33a5924e5e3db62aaf12a7bd9ce661ad69d7b6943054dc81df4845a55e6cb697b5589389987ed42f18779?inline=true)

The downloaded file can now be used in a tool such as SMS to create a prescription.

### Management Zones on Desktop <a href="#management_zones_on_desktop" id="management_zones_on_desktop"></a>

To create management zones and subsequent prescription file:

1. Open FieldAgent on your Desktop.
2. Navigate to the field you’d like to create a prescription for.
3. Select the layer you’d like to create a prescription from.
4. Select the Toolbox.
5. Select the Gears icon.
6. A popup window will indicate loading status. Note that this process may take some time.&#x20;

<figure><img src="https://support.sentera.com/galleryDocuments/edbsn59bc93adbb84bf135987ff24c3cd899ac3692baeb468a547dc3fd963e03c4f9ec4ef5a971975499d97eac500a2c2c509?inline=true" alt=""><figcaption></figcaption></figure>

7. A prescription can then be created. Re-open the toolbox and select the RX icon.
8. Set the units and rate at which the file should be written for.&#x20;

<figure><img src="https://support.sentera.com/galleryDocuments/edbsn1fc6f2b19d8dc3c971cb249de300d6e7e688fe78ac335f66c09c4b6fa4685d2f8949720113548154c904c01a1da2a871?inline=true" alt=""><figcaption></figcaption></figure>

### Area Isolation Example <a href="#area_isolation_example" id="area_isolation_example"></a>

To write a prescription for only the worst or best areas of a field use the toolbox to manipulate the dataset before running the management zone tool. Isolate a specific part of the field by setting the bins to 1 and then drag the min and max sliders around on the graph.

<figure><img src="../../.gitbook/assets/image (503).png" alt=""><figcaption></figcaption></figure>

Settings for this example:

1. Bins were set to 1\
   ![](https://support.sentera.com/galleryDocuments/edbsnb8850057f68a0baeb001425d919f3a4014f1ffe4193e6370f7de0139d2146650a8bef2222e7ea9af897418c0e92c4b73?inline=true)
2. Color Map set to Reds\
   ![](https://support.sentera.com/galleryDocuments/edbsnc1e88bf3868f8b2bbbc3fb04b71737e680615a0e9d48b2e7e22a8fcd7526a6fbdde85be0ffd364f60e9cfcf20d63b2f7?inline=true)
3. Max slider moved to the left\
   ![](https://support.sentera.com/galleryDocuments/edbsn8d46b67b11f07fe8ae8b3f2b54404047240e12b492ff5715143a12de4133cd836884a90d3eb46fecba7e93050850cea2?inline=true)
4. Generate a management zone by pressing the gear icon in the toolbox <img src="https://support.sentera.com/galleryDocuments/edbsnb8850057f68a0baeb001425d919f3a40b300f6940d3aba0b3bdb3d2eaabe1715825a53d7e95826a0bab0a1dac418aa63?inline=true" alt="" data-size="line">

In this case, the worst performing areas of the field were isolated for treatment.

![](https://support.sentera.com/galleryDocuments/edbsn4c492f3582175afca62e4c09172825e006e32486d115e9e95f59780490ed2681f0fd374f81d7bc133a666b4e1f0af00b?inline=true)
