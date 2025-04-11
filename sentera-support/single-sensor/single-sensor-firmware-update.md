# Single Sensor Firmware Update

<img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:blue;">The most recent version of firmware for the Sentera Single Sensor (v2.7.0) is required for the Fly Forward Update. Released March 2022.</mark>

There are two options for updating firmware on the Single Sensor. Option one is the prefered method.

## Option 1: Updating through FieldAgent Desktop |                  <mark style="background-color:green;">Preferred Method</mark> <a href="#option_1_updating_through_fieldagent_desktop__preferred_method" id="option_1_updating_through_fieldagent_desktop__preferred_method"></a>

<img src="https://img.zohostatic.com/zde/static/images/info.png" alt="" data-size="line"> <mark style="background-color:blue;">If you do not have the FieldAgent Desktop App, you can download it here:</mark>\
[<mark style="background-color:blue;">FieldAgent Desktop Download</mark>](http://installs.sentera.com/fieldagent/index.html)

**To upgrade the firmware on your Sentera Single Sensor Through FieldAgent Desktop:**

1. Remove the MicroSD card from your sensor and insert it into a computer running FieldAgent™.\
   <mark style="color:red;">If you are using a new SD Card, ensure the card is formatted to FAT32.</mark> [FAQ: How to update to FAT32](https://support.sentera.com/portal/en/kb/articles/formatting-sentera-mi).
2. Log in to FieldAgent on your desktop computer.
3. Click the gear icon in the upper right and click Update Sentera Camera.
4. Follow the prompts within FieldAgent to complete the process.
5. Insert the MicroSD card back into the sensor.
6. Power on the drone and wait 3 minutes for the firmware update to complete.

## Option 2: Manual Update Process |                                              <mark style="background-color:green;">Without FieldAgent Desktop</mark> <a href="#option_2_manual_update_process__without_fieldagent_desktop" id="option_2_manual_update_process__without_fieldagent_desktop"></a>

**To manually upgrade the firmware on your Sentera Single Sensor, without using FieldAgent Desktop:**

1. Remove the MicroSD card from your sensor and insert it into a computer.\
   <mark style="color:red;">If you are using a new SD Card, ensure the card is formatted to FAT32.</mark> [FAQ: How to update to FAT32](https://support.sentera.com/portal/en/kb/articles/formatting-sentera-mi).
2. Download the firmware file. Link: [Single Firmware v2.7.0](https://docs.zohopublic.com/file/hifsv1e474f86445244c8ab04d102e4512814).
3. Double-click on the downloaded file in a file browser.
4. Select Extract.
5. When prompted to select a destination, click Browse.\


<div align="left"><figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure></div>

6. Choose the SD Card as the destination (_do not select a folder)_, and then click Select Folder.\


<div align="left"><figure><img src="../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure></div>

7. Select Extract or Okay and wait for the extraction process to complete. The firmware folder of the SD card should now look similar to the following:

<figure><img src="../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

8. Insert the MicroSD card back into the Single Sensor.
9. Power on the drone and wait 3 minutes for the firmware update to complete.

## Verify Successful Update (Check Firmware Version) <a href="#verify_successful_update_check_firmware_version" id="verify_successful_update_check_firmware_version"></a>

**To verify the update was successful, check the firmware version:**

1. Remove the MicroSD card from your sensor and insert it into a computer.
2. Open a file browser window and locate the SD Card.
3. Open the folder titled info.\


<figure><img src="../../.gitbook/assets/1 (2).png" alt=""><figcaption></figcaption></figure>

4. Open the file titled firmware-version.txt. Right-click and select Open with and Notepad, if necessary.\


<figure><img src="../../.gitbook/assets/2 (1).png" alt=""><figcaption></figcaption></figure>

5. Check the Firmware version. The top line will indicate the version of firmware currently loaded on the sensor. The second line will indicate the time of the last update.\
   If your sensor is not updating as expected, please contact support for assistance.\


<figure><img src="../../.gitbook/assets/3 (1).png" alt=""><figcaption></figcaption></figure>

## How to Find the Current Version of Firmware on a Sensor via an Image <a href="#how_to_find_the_current_version_of_firmware_on_a_sensor_via_an_image" id="how_to_find_the_current_version_of_firmware_on_a_sensor_via_an_image"></a>

1. Browse to an image file.&#x20;
2. Right-click and select Properties.&#x20;
3. Select the Details tab.&#x20;
4. Scroll to Program Name to view the version number, as shown in the following image.&#x20;

<div align="left"><img src="https://support.sentera.com/galleryDocuments/edbsna77f88b25e8a3a38a3303fe781631a70c80bf6a48a72b3ae2ff00409f3a110f563b6138bffe2550ed69534637bf6c260?inline=true" alt=""></div>
