# Double 4K - Firmware Release Notes

<img src="https://img.zohostatic.com/zde/static/images/file.png" alt="" data-size="line"> <mark style="background-color:yellow;">**Note: Double 4K - Skyport is formerly known as AGX710.**</mark>&#x20;

### Version 1.5.2 | March 30, 2023 <a href="#version_152__march_30_2023" id="version_152__march_30_2023"></a>

#### Features <a href="#features" id="features"></a>

For S/N's 200+: Add support for Mavic 3E systems (912600 baud U-blox)

Add support for U-blox Gen-9 in PHX

Inhibit Skyport triggers when operating in non Command trigger mode

Update branding on configuration page

Use RTK data over Skyport for supported platforms and configurations

Additional logging of Skyport position data per session

#### Bug Fixes <a href="#bug_fixes" id="bug_fixes"></a>

Fix issue preventing DJI Pilot from updating photo counter

Update location of serial number tag to more standard id

Add missing band information for some D4k Variants (-10, -11, -98, etc)

***

### Version 1.4.0 <a href="#version_140" id="version_140"></a>

#### Features <a href="#features_1" id="features_1"></a>

Add XMP::Sentera tags to indicate the home takeoff location, altitude, and accuracy.

Default to assume forward facing flight on DJI Phantom/Mavic/Inspire systems.&#x20;

***

### Version 1.3.1 <a href="#version_131" id="version_131"></a>

#### Features <a href="#features_2" id="features_2"></a>

Add support for different gimbal processors.&#x20;

***

### Version 1.3.0 <a href="#version_130" id="version_130"></a>

#### Features <a href="#features_3" id="features_3"></a>

Enabled support for non-east facing flights.

#### Bug Fixes <a href="#bug_fixes_1" id="bug_fixes_1"></a>

Fixed issues with restarting sessions midflight.

Improved attitude stabilization.

Improved logging.

Fixed issue where above ground altitude was not written to image tags.

Fixed incorrect determination of terrain estimate.&#x20;

Fixed issue that prevented gimbal firmware from updating.&#x20;

Fixed issue on PHX RTK payloads recording incorrect terrain altitude.

Fixed incorrect terrain if AGX gimbal is launched prematurely.

***

### Version 1.2.1 <a href="#version_121" id="version_121"></a>

#### Bug Fixes <a href="#bug_fixes_2" id="bug_fixes_2"></a>

Fix missing ACK packets for SCCP Protocol.

***

### Version 1.2.0 <a href="#version_120" id="version_120"></a>

#### Features <a href="#features_4" id="features_4"></a>

Updated exposure on select cameras for improved image analytics processing.

Added exposure information to exif and XMP:

Exif:ExposureBiasValue - EV Value target for the image.&#x20;

XMP:Sentera:ExposureTarget - The value in the config file for EV (-12 to 12).

Added option to change which camera is used for overlap calculations:

Defaults to widest field of view camera.

#### Bug Fixes <a href="#bug_fixes_3" id="bug_fixes_3"></a>

Fixes for switching camera streams on AGX710 Skyport video.

***

### Version 1.1.1 <a href="#version_111" id="version_111"></a>

#### Bug Fixes <a href="#bug_fixes_4" id="bug_fixes_4"></a>

Fix invalid session.txt altitude on PHX if camera reboots during launch

Set xmp IsNormalized=0 for better Pix4D support

***

### Version 1.1.0 <a href="#version_110" id="version_110"></a>

#### Features <a href="#features_5" id="features_5"></a>

Add fallback to platform GPS on RTK GPS dropout

***

### Version 1.0.3 <a href="#version_103" id="version_103"></a>

#### Bug Fixes <a href="#bug_fixes_5" id="bug_fixes_5"></a>

AGX: Fix compatibility issues with newest M2XX firmware

***

### Version 1.0.2 <a href="#version_102" id="version_102"></a>

#### Bug Fixes <a href="#bug_fixes_6" id="bug_fixes_6"></a>

AGX: Fix update issues on some AGX Platforms

***

### Version 1.0.1 <a href="#version_101" id="version_101"></a>

#### Features <a href="#features_6" id="features_6"></a>

Add system information to the diagnostics web page with firmware and hardware details

#### Bug Fixes <a href="#bug_fixes_7" id="bug_fixes_7"></a>

Fixed RTP video streams not starting properly

Fix camera hanging when AGX payloads did not detect a co-processor

***

### Version 1.0.0  <a href="#version_100" id="version_100"></a>

#### Features <a href="#features_7" id="features_7"></a>

config.yml files are now removed from the MicroSD card after being stored internally in the camera

This allows swapping cards between cameras without modifying their config files

The current config and factory defaults are now found in the /info folder

To apply an update, copy the config.yml from the info folder to the root, modify the file, and reboot

If the config fails to load, it will be renamed to .failed along with a reason for the failure

Improved error messages to the user can be found on the camera web page

Information on the camera hardware is written to /info/hardware-config.yml on boot

Added capability for custom UV filters / aggressive CAC for tower inspections

AGX system/gimbal firmware now automatically updated to match camera firmware

#### Bug Fixes <a href="#bug_fixes_8" id="bug_fixes_8"></a>

Fix for custom (XXXXX-99) cameras video feeds

I2C fixed for 6601 to support light sensors

Loss of communication with the camera now display Communication Lost rather than SDCard missing

***

### Version 0.26.0 <a href="#version_0260" id="version_0260"></a>

#### Features <a href="#features_8" id="features_8"></a>

Improvements to LiveAnalytics for Stand Count

Added M200/M210 V2 Video Feed Support

***

### Version 0.25.2 <a href="#version_0252" id="version_0252"></a>

#### Bug Fixes <a href="#bug_fixes_9" id="bug_fixes_9"></a>

Fix for the rare occurrence of corrupt images due to large thumbnail sizes&#x20;

***

### Version 0.25.1 <a href="#version_0251" id="version_0251"></a>

#### Features <a href="#features_9" id="features_9"></a>

Added AGL Altitude to XMP.Camera.AboveGroundAltitude

Always write band information for cameras (removed option from the config file)

For S/N's 001 - 199: Update LEDs to be solid red/green = no go/go

#### Bug Fixes <a href="#bug_fixes_10" id="bug_fixes_10"></a>

AGX710: Fixed LiveNDVI view on Analytics cameras

Improved accuracy of LiveNDVI calculations for all sensors

***

### Version 0.25.0 <a href="#version_0250" id="version_0250"></a>

#### Features <a href="#features_10" id="features_10"></a>

For S/N's 200+: Add BLE support for setting overlap via Field Agent App

For S/N'S 200+: Update LED status codes to simpler Red/Green NoGo/Go

***

### Version 0.24.0 <a href="#version_0240" id="version_0240"></a>

#### Features <a href="#features_11" id="features_11"></a>

For S/N's 001 - 199: Added Analytics support

For S/N's 200+: Improved analytics processing time by a factor of 2

***

### Version 0.23.2 <a href="#version_0232" id="version_0232"></a>

#### Features <a href="#features_12" id="features_12"></a>

Enhanced RGB image quality and exposure settings.

Improved image metadata support for Pix4D.

New DISTANCE\_3D trigger mode for vertical inspection applications.

AGX710 specific updates.

Enabled live analytics (stand and weed counts) for supported variants.

Fixed M200/M210 flight stability while connected to the Skyport.

Improved gimbal pointing performance.\


***

### Version 0.21.1 <a href="#version_0211" id="version_0211"></a>

#### Bug Fixes <a href="#bug_fixes_11" id="bug_fixes_11"></a>

AGX710: Fixed XMP Wavelength information generation for multispectral systems

***

### Version 0.21.0 <a href="#version_0210" id="version_0210"></a>

#### Features <a href="#features_13" id="features_13"></a>

AGX710: Camera will power down and close the sdcard on drone power off

AGX710: GPS Time used for timestamp rather than unreliable app time

Note: Existing customers will have to update SessionType to TIME\_FIX to use this

AGX710: Altitude will be recorded as MSL instead of AGL in metadata files

AGX710: DJI Pilot widgets for selecting camera stream will reflect the actual imager types

***

### Version 0.20.3 <a href="#version_0203" id="version_0203"></a>

#### Bug Fixes <a href="#bug_fixes_12" id="bug_fixes_12"></a>

Corrected an issue with Deere RTK systems that would report incorrect MSL altitudes

***

### Version 0.20.2 <a href="#version_0202" id="version_0202"></a>

#### Bug Fixes <a href="#bug_fixes_13" id="bug_fixes_13"></a>

Improved robustness of communication with Deere RTK receivers

***

### Version 0.20.1 <a href="#version_0201" id="version_0201"></a>

#### Bug Fixes <a href="#bug_fixes_14" id="bug_fixes_14"></a>

AGX-710: Fixed an issue with incorrect timestamps when no absolute time is received

***

### Version 0.20.0 <a href="#version_0200" id="version_0200"></a>

#### Features <a href="#features_14" id="features_14"></a>

Add support for John Deere RTK Systems (M210)

More visible errors on web page when SDcard is missing

Added age of corrections display to status webpage for RTK systems

Visible on RTK enabled systems only

Added satellite signal strength to ublox logging

***

### Version 0.19.1 <a href="#version_0191" id="version_0191"></a>

#### Features <a href="#features_15" id="features_15"></a>

Added further XMP tag support for Pix4D

Band width/frequencies and color transformation matrices

Add Z offset for antennae on RTK systems

#### Bug Fixes <a href="#bug_fixes_15" id="bug_fixes_15"></a>

Fixed a bug preventing quicktiles from PHXPro RTK systems

***

### Version 0.19.0 <a href="#version_0190" id="version_0190"></a>

#### Features <a href="#features_16" id="features_16"></a>

Add support for Sentera PHX RTK Revision 2 Payloads (Mavlink over UDP)

Add support for M200 Series gimbaled payloads (DJI PSDK)

Photo mode and Video clip recording from DJI Pilot is supported

Streaming Video, LiveNDVI, and Camera Switching available in DJI Pilot

FieldAgent Mobile support for image feedback

Add support for metadata from Honeywell Hg4940 series Inertial Navigation Systems

Add ability to set baud rate for all serial port protocols from the config file

Allows Mavlink interfaces to run at their default 57600 bps

Allow all protocols to interface over serial or UDP

DJI API Port (M100/A3) is currently not supported over serial

#### Bug Fixes <a href="#bug_fixes_16" id="bug_fixes_16"></a>

Fixes inability to start session on Omni-RTK Piksi Systems

#### Misc <a href="#misc" id="misc"></a>

New config.yml structure, old files will be automatically upgraded on boot

config.yml Version 1.3

***

### Version 0.18.2 <a href="#version_0182" id="version_0182"></a>

#### Features <a href="#features_17" id="features_17"></a>

Adds support for Sentera PHX RTK Camera Payloads

SourceType: MAVLINK\_SBP

#### Bug Fixes <a href="#bug_fixes_17" id="bug_fixes_17"></a>

Fixes communication with M100/M600 platforms broken by newer firmware updates

Fixes incorrect setting for GPU governor on bootup

***

### Version 0.18.1 <a href="#version_0181" id="version_0181"></a>

#### Bug Fixes <a href="#bug_fixes_18" id="bug_fixes_18"></a>

Fixed session start issues with Omni and PHX Pro platforms

***

### Version 0.18.0 <a href="#version_0180" id="version_0180"></a>

#### Features <a href="#features_18" id="features_18"></a>

Added support for Swift Piksi RTK GPS units on M100 systems

Enabled world file usage for DJI/Inspire systems

For best results, use an Inspire system with a NADIR Gimbal

Added iperf3 server to test connection quality to the camera

Increased precision of lat/long EXIF tags to allow for RTK precision

Auto ISO is now enabled for use on all cameras.

This will auto-adjust gain to a max shutter speed of 2.5ms

Decreased key-frame interval on video feed to improve performance in lossy datalinks

Added detailed payload attitude support for Sentera gimbals on Indago2 firmware >2.7.0

All platform types now record GPS accuracy and details in XMP or EXIF tags when the information is available.

Added support to enable/disable wifi access point from the config file (Requires installed wifi antennas)

SSID: Sentera\_\[PartNumber]\_\[SerialNumber]

ex. Sentera\_21020-03\_0003

Pass: \[SerialNumber]\[SerialNumber]

ex. 00030003

Added improved web page interface

GPS position, status, and attitude data can now be monitored

Configuration files can be swapped

Popular config files can now be stored internally in the camera (or SDcard) and selected via the web interface.

#### Bug Fixes <a href="#bug_fixes_19" id="bug_fixes_19"></a>

Imagers now consistently take images in the same order, improving high overlap surveys

Fixed a bug that was preventing the info.txt file from being generated in some case

Fixed XMP import issues with newer versions of Pix4D

Improved behavior of the system during overheat conditions

***

### Version 0.17.0 <a href="#version_0170" id="version_0170"></a>

#### Features <a href="#features_19" id="features_19"></a>

Added support for FieldAgent™ ILS Analysis

Added thermal and CPU performance logs to the info folder to monitor thermal issues

Added Mavlink message logging

Added capability to disable CPU cores

#### Bug Fixes <a href="#bug_fixes_20" id="bug_fixes_20"></a>

If no firmware folder is present on the SDcard, an empty folder is created

GPS Latitude and Longitude Exif tags updated to be unsigned rationals

A missing SDcard will still allow the system to boot (but not start a session)

***

### Version 0.16.1 <a href="#version_0161" id="version_0161"></a>

#### Bug Fixes <a href="#bug_fixes_21" id="bug_fixes_21"></a>

Improved capture rate while using XMP tags in images

Fixed a possible crash when capturing images at near the max rate of the camera

***

### Version 0.16.0 <a href="#version_0160" id="version_0160"></a>

#### Features <a href="#features_20" id="features_20"></a>

Added Support for Narrowband NDRE, NDVI, and RGB Filters

#### Bug Fixes <a href="#bug_fixes_22" id="bug_fixes_22"></a>

Copying firmware update files to the SDCard on MaxOSX now updates properly

***

### Version 0.15.2 <a href="#version_0152" id="version_0152"></a>

#### Bug Fixes <a href="#bug_fixes_23" id="bug_fixes_23"></a>

Fixed bug preventing ILS over UDP from starting a session

***

### Version 0.15.1 <a href="#version_0151" id="version_0151"></a>

#### Bug Fixes <a href="#bug_fixes_24" id="bug_fixes_24"></a>

Fix attitude in Ublox based systems (Phantom/Inspire Upgrades)

Disable Auto Antibanding for all imagers

***

### Version 0.15.0 <a href="#version_0150" id="version_0150"></a>

#### Features <a href="#features_21" id="features_21"></a>

Additional XMP and Exif tags are now written to jpeg images

pix4d.csv is no longer required to import into Pix4D, all camera parameters, GPS, and pose are contained in the image

Cameras with supported hardware now perform flat field corrections on the camera before saving the image

Omni systems can now control the EV Compensation and ISO in flight with OSD feedback

***

### Version 0.14.0 <a href="#version_0140" id="version_0140"></a>

#### Features <a href="#features_22" id="features_22"></a>

Onboard FFC is enabled for select Snapcam hardware

Improved timing repeatability across the board when triggering near the maximum camera rate

Thumbnails are not longer embedded in exif (they were not being used)

Light Sensor and GPS/RTK Precision data is now recorded to image-metadata.txt

Dji.csv log file now generated with information received from DJI autopilots

#### Bug Fixes <a href="#bug_fixes_25" id="bug_fixes_25"></a>

If the hardware-config partition is corrupt, a better log message is generated

***

### Version 0.13.3 <a href="#version_0133" id="version_0133"></a>

#### Bug Fixes <a href="#bug_fixes_26" id="bug_fixes_26"></a>

Closing a session without a video feed will now complete successfully

***

### Version 0.13.2 <a href="#version_0132" id="version_0132"></a>

#### Features <a href="#features_23" id="features_23"></a>

Added CPU temperature and frequency logging to jpegs.csv

***

### Version 0.13.1 <a href="#version_0131" id="version_0131"></a>

#### Bug Fixes <a href="#bug_fixes_27" id="bug_fixes_27"></a>

A3 Support over UDP works in DJI Simulator again

***

### Version 0.13.0 <a href="#version_0130" id="version_0130"></a>

#### Features <a href="#features_24" id="features_24"></a>

Added a new overlay to indicate the pitch and roll of the gimbal

A line with degree markers is shown at -90, 0, and 90 degrees absolute to help with inspection

Added a System Time packet to the ICD to allow fine tuning of time before and during a session

See ICD Documentation for more details

Many improvements to how the config.yml file is handled

The last known good config file is now saved in the camera and used if config.yml on the card is blank or missing

A factory config file can be set for the camera to use as a reference. This file is written out to the SDcard on boot

config.yml is always written to the SDCard on boot if the card is present. This allows the user to see what settings are loaded

#### Bug Fixes <a href="#bug_fixes_28" id="bug_fixes_28"></a>

Fixed a bug in the Still Session Ack Packet that was sending an incorrect ID

Fixed a bug where autopilots without attitude

Blank config files will no longer crash the camera

***

### Version 0.12.2 <a href="#version_0122" id="version_0122"></a>

#### Features <a href="#features_25" id="features_25"></a>

Added Hardware Configuration files containing Imager.confs

IMPORTANT: These will need to be loaded in after the firmware going forward from this version

System.info files now saved to image folders as well and imported into FieldAgent™.

LiveNDVI cameras report as NIR+ in ICD Status Packets

#### Bug Fixes <a href="#bug_fixes_29" id="bug_fixes_29"></a>

Fixed a bug where changing video feeds could cause the feed to crash

***

### Version 0.12.1 <a href="#version_0121" id="version_0121"></a>

#### Features <a href="#features_26" id="features_26"></a>

Added logging of RTK Relative Position to gps.csv

#### Bug Fixes <a href="#bug_fixes_30" id="bug_fixes_30"></a>

Increased readability of yellow GPS Status Icons (Darker Shade)

Fixed factor offset in gps.csv log file

***

### Version 0.12.0 <a href="#version_0120" id="version_0120"></a>

#### Features <a href="#features_27" id="features_27"></a>

Added GPS Status Overlay to video feed

Added Crosshairs to video feed

Added capability to disable individual OSD items

Added StartingZoomSteps config to start the camera zoomed in for factory focusing

#### Bug Fixes <a href="#bug_fixes_31" id="bug_fixes_31"></a>

Fixed a color mapping bug for LiveNDVI that was resulting in bad images

***

### Version 0.11.0 <a href="#version_0110" id="version_0110"></a>

#### Features <a href="#features_28" id="features_28"></a>

Added support for Ublox over UDP configuration for the OMNI platform

Added support for OMNI metadata using combined Ublox (Lat/Long/Height) and DJI (Yaw)

This mode is selected with Source Type: &#x55;_&#x42;LO&#x58;_&#x50;\_DJI

#### Bug Fixes <a href="#bug_fixes_32" id="bug_fixes_32"></a>

Time Interval of < 1 second for triggers is now interpreted correctly

Fixed ICD for ImagerPreviewStream setup to correct an RGB/NDVI selection issue

ICD Status packets now report the correct imager type following the Sentera ICD.

Changed Height for Ublox to use hMSL rather than height above ellipsoid.

Fixed a gimbal lock issue when calculating image roll/pitch/yaw at a gimbal position of exactly 90

#### Known Issues <a href="#known_issues" id="known_issues"></a>

Occasionally, the config.yml on the SDcard can be erased. When this happens, the LED will remain blinking red and never go green.

To fix the boot issue, copy the backup file on the SDcard to config.yml replacing the bad one.

***

### Version 0.10.0 <a href="#version_0100" id="version_0100"></a>

#### Features <a href="#features_29" id="features_29"></a>

A3 GPS Detail packet parsing added to get MSL altitude and other useful parameters

Parsing of SBGC data for the Omni and M600 systems added

Source type for DJI and U\_BLOX modes can now also be commanded

***

### Version 0.9.1 <a href="#version_091" id="version_091"></a>

#### Bug Fixes <a href="#bug_fixes_33" id="bug_fixes_33"></a>

Fixed minor threading issues when opening and closing sessions frequently during a flight

***

### Version 0.9.0 <a href="#version_090" id="version_090"></a>

#### Features <a href="#features_30" id="features_30"></a>

Support for DJI-M100 platform added

Uses Lat/Long/Alt/Yaw/Flight Status from the SDK

Support for DJI-M600 platform added

Uses Lat/Long/Alt/Yaw/Time/Flight Status from the SDK

Added user adjustable autoexposure settings.

Can choose: frame-average, center-weighted, spot-metering

Added a picture taken OSD indicator to the upper right corner of the video stream

Camera Preview Setup packet form the ICD support is now added, with new fields appended for preview stream position and OSD enable/disable

Digital Camera Zoom now supported through the ICD

Session.txt support added offline QuickTiles

Overlap modes are supported as a trigger mode for the M100/600 platforms

Support added for Incident Light Sensors over UDP

#### Bug Fixes <a href="#bug_fixes_34" id="bug_fixes_34"></a>

The system will now only queue up to 5 triggers if it is flooded with trigger requests at a rate faster than it can handle (usually > 2Hz). Any trigger requests given after the queue has reached 5 will be ignored and logged as a failed trigger.

World projection files in PROCERUS mode (Kestral Autopilot / ICD) now use aircraft yaw when generating world files.

Terrain Elevation packets will now update the terrain estimate used for automatic overlap modes.

Improved error handling when the IMU is not present on the I2C bus

#### Known Issues <a href="#known_issues_1" id="known_issues_1"></a>

Auto Overlap Trigger Modes do not currently take into account the digital zoom level

***

### Version 0.8.4 <a href="#version_084" id="version_084"></a>

#### Bug Fixes <a href="#bug_fixes_35" id="bug_fixes_35"></a>

Fix for Mavlink Altitude being reported as too low in the metadata files

***

### Version 0.8.3 <a href="#version_083" id="version_083"></a>

#### Bug Fixes <a href="#bug_fixes_36" id="bug_fixes_36"></a>

Fix the RTP Header for Mpeg2 TS w/ RTP Headers

***

### Version 0.8.2 <a href="#version_082" id="version_082"></a>

#### Bug Fixes <a href="#bug_fixes_37" id="bug_fixes_37"></a>

Fix for incorrect time being received over Mavlink packets

***

### Version 0.8.1 <a href="#version_081" id="version_081"></a>

#### Bug Fixes <a href="#bug_fixes_38" id="bug_fixes_38"></a>

Fixed a crash when using Mpeg2\_TS in very bright or very dark environments

***

### Version 0.8.0 <a href="#version_080" id="version_080"></a>

#### Features <a href="#features_31" id="features_31"></a>

Added Mpeg2 Transport Stream as an option for streaming video

New config options to support RTP/Raw for H264 and Mpeg2\_TS

Config file can now control whether live ndvi is used or not for streaming video

#### Bug Fixes <a href="#bug_fixes_39" id="bug_fixes_39"></a>

FOV in the status packet is now set to the value found in the config.yml

***

### Version 0.7.1 <a href="#version_071" id="version_071"></a>

#### Features <a href="#features_32" id="features_32"></a>

IMU Attitude data added to imu.csv for testing

#### Bug Fixes <a href="#bug_fixes_40" id="bug_fixes_40"></a>

Fixed Yaw/Pitch/Roll data in image metadata for Kestral autopilots

Fixed timestamps in metadata for Kestral autopilots

Session.txt files now correctly generated for offline QuickTile in FieldAgent™

Fixed status update rate to match VCHeavy refresh

Change heading names in a number of log files to correctly reflect timestamp values

***

### Version 0.7.0 <a href="#version_070" id="version_070"></a>

#### Features <a href="#features_33" id="features_33"></a>

Added capability to set the EV and ISO in the config file

snapcam.sdp is now automatically recreated when specifying new port/IP address for the video

Added capability to disable/enable video streaming and recording

Added capability to set status/video packets to a multicast IP

Added 2 new GPS trigger modes, GPS Automatic Overlap, and Fixed Height Overlap

#### Bug Fixes <a href="#bug_fixes_41" id="bug_fixes_41"></a>

Fixed the video being mirrored compared to the vehicle and jpeg images

***

### Version 0.6.1 <a href="#version_061" id="version_061"></a>

#### Bug Fixes <a href="#bug_fixes_42" id="bug_fixes_42"></a>

Fixed a crash that could occur when triggering during session initialization

Removed a comma from the ILS log header

***

### Version 0.6.0 <a href="#version_060" id="version_060"></a>

#### Features <a href="#features_34" id="features_34"></a>

Terrain and Altitude (0x0E Packet) Support Added

Session.txt to allow offline QuickTiles added

EPSG.txt file now generated in the base directory when creating world files

Updated support for new light sensor board (TCS34715)

#### Bug Fixes <a href="#bug_fixes_43" id="bug_fixes_43"></a>

Fixed a compatibility issue with the new ICD and old Kestral autopilots. There is now an option to use the older Revision R protocol for these systems.

***

### Version 0.5.1 <a href="#version_051" id="version_051"></a>

#### Bug Fixes <a href="#bug_fixes_44" id="bug_fixes_44"></a>

Fixed a compatibility bug with session ACK and VCTouch preventing session starts

***

### Version 0.5.0 <a href="#version_050" id="version_050"></a>

#### Features <a href="#features_35" id="features_35"></a>

Added logging of system messages to /info/logs (record of last 10 boots)

Configuration data used to capture images is saved for each session in session.info

Incident Light Sensor Support Added

Session Start and Triggering Modes are now separate

Camera and file creation times are now set by the GPS or Autopilot when available

Periodic capture mode is available as a trigger mode

GPS Accuracy required to start a session in GPS\_FIX mode can now be set

Session name conflicts no longer override data

Append session options from ICD will now work. If the same session name plus the append flag is set, images will be appended to the session.

The default behavior without the flag is to append _### to the end of the identical session name. eg if 'test' already exists and append is off, starting a new session with this name will result in the folder 'tes&#x74;_&#x30;01', then 'test\_002', etc

#### Bug Fixes <a href="#bug_fixes_45" id="bug_fixes_45"></a>

Opening a session when one is already open will now work

If the session is already open with the same name, the command is ignored

If the session name is different, the current session is closed and a new one opens.

The camera will again listen for multicast packets for ICD commands.

Fixed an issue that would cause ICD packets to get cross when rapid commands were issued.

***

### Version 0.4.1 <a href="#version_041" id="version_041"></a>

#### Features <a href="#features_36" id="features_36"></a>

From this release onwards, version downgrades are allowed by default

Added an option to disable world file generation

Allow the user to set a fixed altitude for world file generation

Allow the user to set the GPS trigger distance

GPS.csv is now generated when using Ublox GPS

Allows customization of the IP and port numbers for the system components

#### Bug Fixes <a href="#bug_fixes_46" id="bug_fixes_46"></a>

Fixed a bug that was causing NIR image to be encoded in software causing excessive CPU usage

***

### Version 0.4.0 <a href="#version_040" id="version_040"></a>

#### Features <a href="#features_37" id="features_37"></a>

Initial support for Mavlink Added

#### Bug Fixes <a href="#bug_fixes_47" id="bug_fixes_47"></a>

Default Video Size changed to 1920x1080

Fixed missing busybox commands from build 0.3.0

#### Known Issues <a href="#known_issues_2" id="known_issues_2"></a>

Mavlink does not currently work with Mission Planner

2 Vehicles are detected, does not trigger

***

\


### Version 0.3.0 <a href="#version_030" id="version_030"></a>

#### Features <a href="#features_38" id="features_38"></a>

Configuration file added to allow user control of settings

External GPS Can now trigger images

Live Video Streaming during an active session is now enabled

Top/Bottom, PiP, and Fullscreen modes available

Projection files are now generated for each image

HTTP Server added to browse folders, latest image, and current session files

#### Bug Fixes <a href="#bug_fixes_48" id="bug_fixes_48"></a>

VC Touch "Snapshot" Button Support

Color Conversion from YUV to RGB fixed

***

### Version 0.2.0 <a href="#version_020" id="version_020"></a>

#### Notes <a href="#notes" id="notes"></a>

Initial Release. This is the first official release and supports ONLY Kestral autopilots. Triggering must be done by the autopilot.

#### Features <a href="#features_39" id="features_39"></a>

Kestral Autopilot Support Added

#### Bug Fixes <a href="#bug_fixes_49" id="bug_fixes_49"></a>

Initial Release

#### Known Issues <a href="#known_issues_3" id="known_issues_3"></a>

Does not currently import into FieldAgent™ (needs more CSV Files)

\
