# Double 4K Sensor Image Capture

## How does my Double 4K Sensor capture images? <a href="#how_does_my_double_4k_sensor_capture_images" id="how_does_my_double_4k_sensor_capture_images"></a>

Sentera Sensors will capture images whenever they are powered on and their trigger conditions are met. This occurs whether you’re flying with FieldAgent Mobile, or any third party application.

## Trigger Conditions <a href="#trigger_conditions" id="trigger_conditions"></a>

There are 4 different modes for trigger conditions, based on overlap, altitude, distance and time values. You can switch between these modes by editing a text file on the sensor's SD card. We will cover how to do that later in this article.

### Auto Height Overlap  <a href="#id-1_auto_heightoverlap" id="id-1_auto_heightoverlap"></a>

Green sensors are set to Auto Height Overlap by default. This mode uses two variables to know when to capture: 'Minimum Trigger Height Above Ground Level' and 'Overlap Percent'.&#x20;

* **Minimum Height:**  When the sensor is below the minimum height, it will not capture images. The sensor's height is determined by its distance above the launch location. A low minimum height value helps reduce the amount of unwanted images taken on the ground and in transit, but it can prevent low altitude image capture. The default value is set to 10 meters. You can change this value to be between 0 and 200 meters.&#x20;
* **Overlap:** The sensor will capture an image once it has moved far enough to achieve the overlap value. The default value is 70%. You can change this value to between -600% and +90% overlap. If you have a Bluetooth enabled sensor, you are able to change the overlap percentage in the app.&#x20;

Once your sensor reaches the minimum height and moves far enough to achieve the set overlap value, it will start capturing images.&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/auto d4k.jpg" alt="" width="314"><figcaption><p><em><mark style="color:blue;">Configuration file for Auto Height Overlap mode on the Double 4K</mark></em></p></figcaption></figure></div>

### Known Height Overlap  <a href="#id-2_known_height_overlap" id="id-2_known_height_overlap"></a>

This mode is similar to auto height overlap, except it requires you to specify what height your drone will be flying at. It uses two variables to know when to capture, 'Known Height Above Ground Level' and 'Overlap Percent'. This mode is useful when flying with Terrain Informed over a hilly field. Terrain Informed flight planning adjusts your drone's altitude to maintain the same distance above the field. By setting a known height above ground, your sensor is able to calculate when to take images, despite the differences in altitude.&#x20;

* **Known Height:** Set this value to the distance above ground your drone will be flying. Make sure this value matches the altitude of your flight plan. If you have an incorrect Known Height value, your sensor will not capture images with the set overlap value. You will need to update this setting every time you to plan to fly a different altitude. You can change this value to between 0 and 400 meters.
* **Overlap:** The sensor will capture an image once it has moved far enough to achieve the overlap value. The default value is 80%, which is recommended to stitch your images. You can change this value to between -600% and +90% overlap. If you have a Bluetooth enabled sensor, you are able to change the overlap percentage in the app.&#x20;

Once your sensor moves far enough to achieve the overlap value it will start capturing images. There is no minimum height which you sensor needs to reach.

<div align="left"><figure><img src="../../.gitbook/assets/manual overlap 2 (1).jpg" alt="" width="227"><figcaption></figcaption></figure></div>

<div align="left" data-full-width="false"><figure><img src="../../.gitbook/assets/time d4k (1).jpg" alt="" width="197"><figcaption><p><em><mark style="color:blue;">Configuration file for Manual Height Overlap mode on the double 4k</mark> </em> </p></figcaption></figure></div>

<img src="https://img.zohostatic.com/zde/static/images/caution.png" alt="" data-size="line">  <mark style="background-color:red;">Low altitude flights can be challenging with the overlap trigger modes. When your drone is low and moving fast, it can be limited by the sensor's shutter speed. This means that once your sensor is able to take another image it will have already moved too far to capture an image with the correct overlap. Flying at lower speeds will allow your sensor to capture the correct overlap.</mark>

### Distance <a href="#id-3_distance" id="id-3_distance"></a>

This mode uses a distance variable to determine when to take an image. The default value is 10 meters, meaning your sensor will capture an image once your drone has moved 10 meters in any horizontal direction. You can change this value to between .5 and 1000 meters.

<div align="left"><figure><img src="../../.gitbook/assets/double distance.jpg" alt="" width="227"><figcaption><p><em><mark style="color:blue;">Configuration file for Distance mode on the double sensor</mark></em> </p></figcaption></figure></div>

### Time  <a href="#id-4_time" id="id-4_time"></a>

This mode uses a time variable to determine when to take an image. The default value is 5 seconds, meaning your sensor will capture an image once every 5 seconds. You can change this value to between 1 and 30 seconds.

<div align="left"><figure><img src="../../.gitbook/assets/time 4k.jpg" alt="" width="188"><figcaption><p><em><mark style="color:blue;">Configuration file for Time mode on the Double 4K sensor</mark></em> </p></figcaption></figure></div>

## Selecting a mode <a href="#selecting_a_mode" id="selecting_a_mode"></a>

You can switch between the 4 different trigger modes, as well as change the settings of each individual mode, by editing text files on the sensor's sd card. The Double 4K has a web interface which enables easy switching between different settings you have saved.

To change the trigger settings on your Sentera Double 4K Sensor:

1. Remove the microSD card from your Sentera Sensor and insert it into your PC.
2. Browse to the file labeled Config.yml. Open it with Microsoft Notepad, Microsoft Word, or any other text editor.
3. Scroll to the bottom of the document and change the 'TriggerType' depending on which mode you want to use. The default value is AUTO\_HEIGHT\_OVERLAP.

<div align="left"><figure><img src="../../.gitbook/assets/type whole.jpg" alt="" width="328"><figcaption></figcaption></figure></div>

4. Change the settings of each individual mode as needed. The setting for Known Height Above Ground Level can be found further up in the document.

<div align="left"><figure><img src="../../.gitbook/assets/1111.jpg" alt="" width="222"><figcaption></figcaption></figure></div>

5. Save the changes and insert the microSD card back into your sensor. The setting will remain unchanged until you manually change it or replace the microSD card.
6. The Double 4K has a web interface which allows you to switch between different configuration files you have saved. This is a quick way to change settings between flights.

<div align="left"><figure><img src="../../.gitbook/assets/default 3.jpg" alt="" width="563"><figcaption><p><mark style="color:blue;">Double 4K Web Interface</mark></p></figcaption></figure></div>

#### <mark style="background-color:blue;">More information can be found in the</mark>[ <mark style="background-color:blue;">Configuration File User Guide</mark> ](https://support.sentera.com/portal/api/kbArticles/280672000033251001/locale/en/attachments/seb352975b8df3d9a4354a6e3c390fe39cffa/content?portalId=edbsndc49af6231b384d609b205eda12b95356310426ab79cfafc2949ad93d787da96\&inline=true) <a href="#more_information_can_be_found_in_the_configuration_file_user_guide" id="more_information_can_be_found_in_the_configuration_file_user_guide"></a>
