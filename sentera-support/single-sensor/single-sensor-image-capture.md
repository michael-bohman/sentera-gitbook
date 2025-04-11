# Single Sensor Image Capture

### How does my Single Sensor capture images? <a href="#how_does_my_single_sensor_capture_images" id="how_does_my_single_sensor_capture_images"></a>

Sentera Single sensors will capture images whenever they are powered on and their trigger conditions are met. This occurs whether you’re flying with FieldAgent Mobile, or any third party application.

## Trigger Conditions <a href="#trigger_conditions" id="trigger_conditions"></a>

There are 4 different modes for trigger conditions, based on overlap, altitude, distance and time values. You can switch between these modes by editing a text file on the sensor's SD card. We will cover how to do that later in this article.

<figure><img src="../../.gitbook/assets/modes single.jpg" alt=""><figcaption><p><mark style="color:blue;">Mode Selection on the single sensor</mark></p></figcaption></figure>

### Auto Overlap  <a href="#id-1_auto_overlap" id="id-1_auto_overlap"></a>

Single sensors are set to Auto Overlap by default. This mode uses two variables to know when to capture: 'Minimum Height Above Home Altitude' and 'Overlap Percent'.&#x20;

* **Minimum Height:**  When the sensor is below the minimum height, it will not capture images. The sensor's height is determined by its distance above the home location. A low minimum height value helps reduce the amount of unwanted images taken on the ground and in transit, but it can prevent low altitude image capture.  The Default Value is 12 Meters. You can change this value to be between 0 and 200 meters. Note that very low altitude flights may produce images that are out of focus.&#x20;
* **Overlap:** The sensor will capture an image once it has moved far enough to achieve the overlap value. The default value is 80%, which is recommended to stitch your images. You can change this value to between -600% and +90% overlap. If you have a Bluetooth enabled sensor, you are able to change the overlap percentage in the app.&#x20;

Once your sensor reaches the minimum height and moves far enough to achieve the set overlap value, it will start capturing images.

<figure><img src="../../.gitbook/assets/overlap new.jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/manual overlap single 2.jpg" alt=""><figcaption><p><mark style="color:blue;">Configuration file for Auto Height Overlap mode on the single sensor</mark></p></figcaption></figure>

### Manual Overlap  <a href="#id-2_manual_overlap" id="id-2_manual_overlap"></a>

This mode is similar to auto overlap, except it requires you to specify what height your drone will be flying at. It uses two variables to know when to capture, 'Manual Overlap Height Above Home Altitude' and 'Overlap Percent'. This mode is useful when flying with Terrain Informed over a hilly field. Terrain Informed flight planning adjusts your drone's altitude to maintain the same distance above the field. By setting a manual height above ground, your sensor is able to calculate when to take images, despite the altitude changes in flight. &#x20;

* **Manual Height:** Set this value to the distance above ground your drone will be flying. Make sure this value matches the altitude of your flight plan. If you have an incorrect Manual Height value, your sensor will not capture images with the set overlap value. You will need to update this setting every time you to plan to fly a different altitude. You can change this value to between 0 and 400 feet. Note that very low altitude flights may produce images that are out of focus.&#x20;
* **Overlap:** The sensor will capture an image once it has moved far enough to achieve the overlap value. The default value is 80%, which is recommended to stitch your images. You can change this value to between -600% and +90% overlap. If you have a Bluetooth enabled sensor, you are able to change the overlap percentage in the app.&#x20;

Once your sensor moves far enough to achieve the overlap value it will start capturing images. There is no minimum height which you sensor needs to reach.

<figure><img src="../../.gitbook/assets/overlap new (1).jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/auto overlap.jpg" alt=""><figcaption><p><mark style="color:blue;">Configuration file for the Manual Height Overlap mode on the single sensor</mark></p></figcaption></figure>

<img src="https://img.zohostatic.com/zde/static/images/caution.png" alt="" data-size="line"> <mark style="background-color:red;">Low altitude flights can be challenging with the overlap trigger modes. When your drone is low and moving fast, it can be limited by the sensor's shutter speed. This means that once your sensor is able to take another image it will have already moved too far to capture an image with the correct overlap. Flying at lower speeds will allow your sensor to capture the correct overlap.</mark>&#x20;

### Distance <a href="#id-3_distance" id="id-3_distance"></a>

This mode uses a distance variable to determine when to take an image. The default value is 10 meters, meaning your sensor will capture an image once your drone has moved 10 meters in any horizontal direction. You can change this value to between .5 and 1000 meters.

<div align="left"><figure><img src="../../.gitbook/assets/single distance.jpg" alt=""><figcaption><p><mark style="color:blue;">Configuration file for Distance mode on the single sensor</mark></p></figcaption></figure></div>

### Time  <a href="#id-4_time" id="id-4_time"></a>

This mode uses a time variable to determine when to take an image. The default value is 2.5 seconds, meaning your sensor will capture an image once every 2.5 seconds. You can change this value to between 1 and 30 seconds.

<div align="left"><figure><img src="../../.gitbook/assets/single time.jpg" alt=""><figcaption><p><mark style="color:blue;">Configuration file for Time mode on the single senso</mark>r</p></figcaption></figure></div>

## Selecting a mode <a href="#selecting_a_mode" id="selecting_a_mode"></a>

To change the trigger settings on your Sentera Single Sensor:

1. Remove the microSD card from your Sentera Sensor and insert it into your PC.
2. Browse to the file labeled UserSettings.txt. Open it with Microsoft Notepad, Microsoft Word, or any other text editor.
3. Change the 'TriggerMode' value to 3, 4, 5 or 6, depending on which mode you want to use. The default value is 5 for Auto Overlap mode.
4. Change the settings of each individual mode as needed.

<figure><img src="../../.gitbook/assets/whole file new.jpg" alt=""><figcaption></figcaption></figure>

5. Save the changes and insert the microSD card back into your sensor. The setting will remain unchanged until you manually change it or replace the microSD card.
