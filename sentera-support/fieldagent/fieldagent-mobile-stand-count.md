# FieldAgent - Mobile Stand Count

## Overview <a href="#overview" id="overview"></a>

<div align="left"><figure><img src="../../.gitbook/assets/Untitled.png" alt="" width="375"><figcaption></figcaption></figure></div>

The Mobile Stand Count feature for FieldAgent Mobile (iOS app) is intended for quickly processing shareable Stand Count results from the field’s edge. The video below shows it populating in real time:&#x20;

<figure><img src="https://lh3.googleusercontent.com/3-GvHfCsOz9i1PjOmCGJjX1sWnM4E3FSGU83_Bgf-gmcxTJWSVptULb4Jo9VJmaozhx_cyZXIVs5odmErw4JiGV5ZRS6vhKFLog6wypb29M7ZVCo5lNTlchFWmFDuS4XYH1v8pGJyFRoP7XkjyJP2g" alt=""><figcaption></figcaption></figure>

A map result will be shareable immediately after processing. Sharing options include text message, iMessage, email, and any other iOS supported applications.

\
Mobile Stand Counts processed on FieldAgent for iOS are run through the same steps as FieldAgent Web and Desktop and thus users can expect the same results.

\
<img src="https://img.zohostatic.com/zde/static/images/file.png" alt="" data-size="line"> <mark style="background-color:yellow;">NOTE: Stand Count on FieldAgent Mobile (iOS app) will not upload the underlying imagery associated with each numbered disc on the map. To attach imagery to the numbered discs, Stand Count must be</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">**reprocessed**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">using FieldAgent on Web or Desktop.</mark>

***

## Requirements

Although there are a few requirements for processing Mobile Stand Counts with FieldAgent Mobile, it is worth noting that **online connectivity is NOT a requirement to generate a stand count\*!** &#x20;

### FieldAgent Subscription Type <a href="#fieldagent_subscription_type" id="fieldagent_subscription_type"></a>

Stand Count on FieldAgent Mobile (iOS app) requires users to have an **Enterprise, Advisor Standard, or Advisor Premium License.**\
\
<img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:blue;">For more information on pricing, view</mark> [<mark style="background-color:blue;">our pricing page</mark> ](https://sentera.com/agronomic-analytics/)<mark style="background-color:blue;">.</mark>

### Sensor

The following sensors are supported:

* Sentera Double 4K Analytics on a DJI M300 or Sentera PHX
* DJI Phantom 4 Pro V2 built in RGB Sensor
* DJI Mavic 2 Pro built-in RGB Sensor
* DJI Mavic 3 Enterprise built-in RGB Sensor

| Sensor                        | Flight Altitude |
| ----------------------------- | --------------- |
| Sentera Double 4K - Analytics | 150ft           |
| DJI Mavic 2 Pro               | 50 ft           |
| DJI Phantom 4 Pro V2          | 50 ft           |
| DJI Mavic 3 Enterprise        | 50 ft           |

### iOS Device

**Mobile Stand Count only works on iPads** . The newer the iOS device, the faster Stand Counts will process.  You will also need a microSD card adapter that is compatible with your iPad.

### Crop Types <a href="#crop_types" id="crop_types"></a>

* Corn
* Cotton
* Potato
* Soybeans

### Crop Size

Plants should be at least 4 inches leaf across, leaf tip to leaf tip. Rowfill mode will be used when plants within a row are touching. Stand Counts can not be performed when the space between rows is covered by crop canopy.

### Uploading (\*online connectivity) <a href="#uploading_online_connectivity" id="uploading_online_connectivity"></a>

The iPad that is generating Mobile Stand Counts must be connected to the internet in order for Stand Count results to be uploaded to the cloud and accessible on the Web and Desktop. A field must also be selected when running Stand Counts so that the Stand Counts have somewhere to upload. File sizes on Stand Counts are designed to be extremely small, so as not to interfere with low data caps or connections in areas with slow connectivity.

***

## How to use

### Flight Planning for DJI Drones on FieldAgent Mobile  <a href="#flight_planning_for_dji_drones_on_fieldagent_mobile" id="flight_planning_for_dji_drones_on_fieldagent_mobile"></a>

After setting an area or line, and camera:&#x20;

Choose the **Stand** preset. This will set the correct altitude for your camera and set the overlap to capture at \~1 stand count per acre.

<div align="left"><figure><img src="../../.gitbook/assets/Untitled (1).png" alt="" width="370"><figcaption></figcaption></figure></div>

The boundary buffer for Stand Counts is set to 100ft. This will cause Stand Counts over small fields (less than 50 acres) to have much less than one Stand Count per acre. Lowering the boundary buffer (as it is safe to do so) will allow the drone to fly closer to the edges of the field and thus capture more of the field.\
\
<img src="https://img.zohostatic.com/zde/static/images/caution.png" alt="" data-size="line">  <mark style="background-color:red;">WARNING: DJI Mavic and Phantom drones are set to fly at 50 feet in order to collect the imagery with the correct resolution. Use caution when flying at low altitudes.</mark>

### Non-Flat Terrain and Obstacles <a href="#non-flat_terrain_and_obstacles" id="non-flat_terrain_and_obstacles"></a>

When flying over non-flat terrain, [Terrain Informed ](https://support.senterasensors.com/fieldagent-mobile-ios/60-second-guides/terrain-informed-flight)Flight Planning should be turned on as well. Note that while processing Mobile Stand Counts does not require an internet connection, planning a terrain informed flight DOES require an internet connection.

<div align="left"><figure><img src="../../.gitbook/assets/Untitled (2).png" alt="" width="375"><figcaption></figcaption></figure></div>

<img src="https://img.zohostatic.com/zde/static/images/caution.png" alt="" data-size="line"> <mark style="background-color:red;">WARNING:  Concave flight boundaries with surrounding trees should be replanned as line missions.</mark>



Look closely at planned flight routes before pressing launch. Some flight patterns over concave flight boundaries may cut through the boundaries. Cutting through the boundary is the most efficient path, but not the safest.\
\
To solve this problem, clear the flight plan and, in the order the drone can safely fly, select all the locations where you would like to capture an image for Mobile Stand Count. Planning flights in this manner also makes it less likely that images are captured over areas where a Stand Count may not be possible (i.e., over terracing or irrigation channels). See below for an example of a custom planned line flight that ensures the drone will not cross over trees while capturing photos.

### Running Mobile Stand Count <a href="#running_mobile_stand_count" id="running_mobile_stand_count"></a>

1. After flight, remove the SD Card from your sensor or drone and insert into an SD card reader attached to your iOS device.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/Untitled (3).png" alt="" width="563"><figcaption></figcaption></figure></div>

2. From the Home Screen, tap the menu option for Dashboard and select **Review Drone Imagery**
3. Select **Allow Access.**

<figure><img src="../../.gitbook/assets/EEEDB9F3-03D0-41C8-8445-A9435E005AED.png" alt=""><figcaption></figcaption></figure>

4. When prompted, select the SD Card in the finder window and then click **Done** .  FieldAgent will automatically search the SD Card for flights. Flights will be organized by date and time with the most recent flights on top.

<div align="left"><figure><img src="../../.gitbook/assets/Untitled (4).png" alt="" width="563"><figcaption></figcaption></figure></div>

<img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:blue;">Unless necessary, select the SD Card name and not a lower level folder.</mark>

5. Select the flight you’d like to run a Mobile Stand Count and then select **Create Report** at the bottom of the screen. If necessary, deselect or other non-RGB takeoffs.

<div align="left"><figure><img src="../../.gitbook/assets/F7E11313-72F7-4C13-92DE-70E3585ADA08.png" alt=""><figcaption></figcaption></figure></div>

6. Confirm the properties and edit as necessary.

<figure><img src="../../.gitbook/assets/E96BE4E8-1CE3-4CE1-965E-F8E6C5B8E191.png" alt=""><figcaption></figcaption></figure>

&#x20;<img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:blue;">U</mark><mark style="background-color:blue;">ploading results to the cloud requires a field selection. Click Field and choose from your list of fields. You may need to switch organizations to find an existing field.</mark>&#x20;

<figure><img src="../../.gitbook/assets/E130957C-12BD-41DF-9546-F97C5E625990.png" alt=""><figcaption></figcaption></figure>

7. Once you’ve confirmed the properties, select **Start**.&#x20;

## Viewing and Analyzing Results <a href="#viewing_and_analyzing_results" id="viewing_and_analyzing_results"></a>

After analyzing a subset of images results will begin to populate on the screen quickly! This video below shows the process in real time:

<figure><img src="https://lh3.googleusercontent.com/3-GvHfCsOz9i1PjOmCGJjX1sWnM4E3FSGU83_Bgf-gmcxTJWSVptULb4Jo9VJmaozhx_cyZXIVs5odmErw4JiGV5ZRS6vhKFLog6wypb29M7ZVCo5lNTlchFWmFDuS4XYH1v8pGJyFRoP7XkjyJP2g" alt=""><figcaption></figcaption></figure>

### Progress Bar <a href="#progress_bar" id="progress_bar"></a>

A progress bar at the bottom of the screen provides an estimate for how much time remains in processing the selected Mobile Stand Count images.

<figure><img src="../../.gitbook/assets/Untitled (5).png" alt=""><figcaption></figcaption></figure>

### Numbered Discs <a href="#numbered_discs" id="numbered_discs"></a>

As images are processed, discs will appear on the screen in place of the white photo-dots at each image location.

<div align="left"><figure><img src="../../.gitbook/assets/Untitled (6).png" alt="" width="539"><figcaption></figcaption></figure></div>

Each Stand Count disc displays the detected number of plants per acre and is colored according to how that number compares to the other Stand Counts on the screen. Dark green indicates a higher Stand Count, red indicates a lower Stand Count.

\
Recoloring of discs happens in real time. In the example below, a Stand Count in the lower right turns from red to orange as more images are processed.



![Showcasing Mobile Stand Count as its processed](https://lh6.googleusercontent.com/E7Vnq7PkfXrjquTH5afZ_QhtYPM31PeP25jG9ZdDJv7I77Nx-N-LrqHX3PCXMP702pjuFQuZd88DT0GN7bMPCVmO8l6zqWIRa_gSHMvcPvgxqzzaH-UJ_wJZQW50ksfakOsM7aSITB7p0-q21Dv72w) ---> ![Showing Mobile StandCount as its processed](https://lh5.googleusercontent.com/W-ta1zq5jbcsG-FHUGkrE_WIvMYTmPbBykapMMRIz-CbFjhLgAwUmczn7zYUcU-BfDhp7dcOIyVHyN97vj1F4Jg7Hw_SVvu6WwBpzZ8UyYJZSuM00Wgzb7IdLrkxe52R52l1CjysUQJyt8he5TEkTg)

The discs can be selected to preview the image at that location. Select a disc and then press the magnifying glass to preview the annotated image at that location full screen.

\
<img src="https://support.sentera.com/galleryDocuments/edbsn5bcd865d6c697290116b35e64362535d49c1152404f53451414ef0f01790986d2b04e809925a56c19d9767405d9df0ba?inline=true" alt="Mobile Stand Count - Preview images" data-size="original">          ![Annotated images for Mobile Stand Count](https://support.sentera.com/galleryDocuments/edbsncf303e8390b9b40a0255c588bcc9563a7ae018ecb80c09d934679a97f5923e53b8ecaae977a3b0584abefaaa907c349d?inline=true)                            &#x20;

## PDF Report <a href="#pdf_report" id="pdf_report"></a>

Stand Counts can be shared as a PDF report after processing.\
\
1\. Click edit report to open the PDF editing feature and share.\
2\. Click the **Add Notes** section and type in any notes you’d like to add to the report.

<div align="left"><figure><img src="../../.gitbook/assets/Picture2.jpg" alt="" width="320"><figcaption></figcaption></figure></div>

3\. When you are done, **click the Share Icon** in the upper right corner and share using your preferred sharing method.

## Accessing Previously Created PDF Reports <a href="#accessing_previously_created_pdf_reports" id="accessing_previously_created_pdf_reports"></a>

1. Click on the **gear settings** icon from any page in the mobile app and then **My Past Surveys** .
2. Select **My Stand Counts.**

<div align="left"><figure><img src="../../.gitbook/assets/E1658598-2D1A-48DF-B012-25AF8B2D17D9.png" alt="" width="563"><figcaption></figcaption></figure></div>

3\. Select the survey date you’d like to view.

<div align="left"><figure><img src="../../.gitbook/assets/Untitled (7).png" alt="" width="563"><figcaption></figcaption></figure></div>

4\. Share the report using the share icon in the lower right corner.

<div align="left"><figure><img src="../../.gitbook/assets/sc3.jpg" alt="" width="563"><figcaption></figcaption></figure></div>

## Sharing to the Cloud <a href="#sharing_to_the_cloud" id="sharing_to_the_cloud"></a>

<img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:blue;">Underlying images will not be uploaded to the cloud. Make sure you import your images to FieldAgent to save and sync the data.</mark>

Sharing to the cloud happens automatically  **when a field was selected before processing and the iPad was connected to the internet when processing was completed.**

Access Stand Counts generated by FieldAgent Mobile in the Web or Desktop by visiting the field page that the Stand Count was associated with and viewing the map layers.

<figure><img src="../../.gitbook/assets/Untitled (8).png" alt=""><figcaption></figcaption></figure>
