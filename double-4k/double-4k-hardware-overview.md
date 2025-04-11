# Double 4K - Hardware Overview

<img src="https://img.zohostatic.com/zde/static/images/file.png" alt="" data-size="line"> <mark style="background-color:yellow;">Note : Double 4K - Skyport is formerly known as AGX710.</mark>&#x20;

## Mechanical CAD Model <a href="#mechanical_cad_model" id="mechanical_cad_model"></a>

A mechanical model of the Double 4k sensor is available for download in STEP file format.

[Sentera Double 4K CAD Model (.step)](https://workdrive.zohoexternal.com/file/grcwy1c04eb13d18046f69d34e1b9e3dc1845)

## Electrical Connectors <a href="#electrical_connectors" id="electrical_connectors"></a>

The following tables list pin descriptions of the camera connectors.  All 3.3V UART and 3.3V I2C interfaces are _not_ 5V tolerant.  For additional detail on camera interfaces, contact Sentera. J10 is a USB 3.0 connector and is only used by Sentera during development and testing.

<div align="left"><img src="https://desk.zoho.com/DocsDisplay?zgId=669162239&#x26;mode=inline&#x26;blockId=bbr0j7ee3ba0f9cbd4ed78c07b0b44d1474bf" alt="Camera Connectors"></div>

\


**J3 - Main Power and Signals**

| Pin | Signal    | Type | Description                                                        |
| --- | --------- | ---- | ------------------------------------------------------------------ |
| 1   | VCC       | PWR  | Camera power input (6V to 26V).                                    |
| 2   | GND       | PWR  | Camera power input (6V to 26V).                                    |
| 3   | (3V3) TXD | O    | 3.3V UART bus.                                                     |
| 4   | (3V3) RXD | I    | 3.3V UART bus.                                                     |
| 5   | VCC\_3V3  | PWR  | 3.3V switched power output - selectable upon request.              |
| 6   | (3V3)SDA  | I/O  | 3.3V I2C bus.                                                      |
| 7   | (3V3)SCL  | I/O  | 3.3V I2C bus.                                                      |
| 8   | EN\_A     | PWR  | 3.3V switched power output (with pin 5) - selectable upon request. |
| 9   | GPIO\_B2  | I/O  | Reserved.                                                          |
| 10  | RSVD      | N/A  | Reserved.                                                          |

Connector: BM10B-GHS-TBT&#x20;

[Mating Connector: GHR-10V-S](https://www.digikey.com/en/products/detail/jst-sales-america-inc/GHR-10V-S/807822)\


**J4 - Ethernet Pin Descriptions**

| Pin | Signal | Description                      |
| --- | ------ | -------------------------------- |
| 1   | TD0P   | Transmit Data+ or BiDirectional. |
| 2   | TD0N   | Transmit Data- or BiDirectional. |
| 3   | TD1P   | Receive Data+ or BiDirectional.  |
| 4   | TD1N   | Receive Data- or BiDirectional.  |
| 5   | TD2P   | Not connected or BiDirectional.  |
| 6   | TD2N   | Not connected or BiDirectional.  |
| 7   | TD3P   | Not connected or BiDirectional.  |
| 8   | TD3N   | Not connected or BiDirectional.  |

Connector: BM10B-GHS-TBT&#x20;

[Mating Connector: GHR-08V-S](https://www.digikey.com/en/products/detail/jst-sales-america-inc/GHR-08V-S/807820)\


**J5 - Auxiliary Power and Signals**

| Pin | Signal    | Type | Description                             |
| --- | --------- | ---- | --------------------------------------- |
| 1   | GND       | PWR  | 3.3V power output.                      |
| 2   | VCC\_3V3  | PWR  | 3.3V power output                       |
| 3   | EN\_B     | PWR  | Regulated 5V power output, up to 500mA. |
| 4   | VCC\_5V0  | PWR  | Regulated 5V power output, up to 500mA. |
| 5   | (3V3)SCL  | I/O  | 3.3V I2C bus.                           |
| 6   | (3V3)SDA  | I/O  | 3.3V I2C bus.                           |
| 7   | (3V3)RX1  | I    | 3.3V UART bus.                          |
| 8   | (3V3)TX1  | O    | 3.3V UART b                             |
| 9   | (3V3) RXD | I    | 3.3V UART bus.                          |
| 10  | (3V3) TXD | O    | 3.3V UART bus                           |
| 11  | GND       | PWR  | Camera power input (6V to 26V).         |
| 12  | VCC       | PWR  | Camera power input (6V to 26V).         |

Connector: BM12B-GHS-TBT&#x20;

[Mating Connector: GHR-12V-S](https://www.digikey.com/en/products/detail/jst-sales-america-inc/GHR-12V-S/807824)\


The camera is able to auto-negotiate the Ethernet speed.  Therefore, only four pins are required for slower 10Base-T or 100Base-T speeds.  All eight pins are required for communication at a 1000Base-T speed.

Typical users will choose either J3 OR J5 depending on their specific installation requirements. Many of the signals are shared between J3 and J5 including the primary input power, UART, and I2C connections.  The following connections are shared between the connectors:

Camera power input (6V to 26V): VCC & GND

J3: pins 1-2&#x20;

J5: pins 11-12&#x20;

3.3V UART bus: RXD & TXD&#x20;

J3: pins 3-4&#x20;

J5: pins 9-10&#x20;

3.3V I2C bus: SCL & SDA&#x20;

J3: pins 6-7

&#x20;J5: pins 5-6

***

## Display Indicators

The camera contains two indicators for providing feedback on the camera’s operation. The indicator closest to the top of the camera identifies camera Power, while the indicator closest to the bottom of the camera identifies camera Status.  Each display indicator contains a set of LEDs: a green LED and a red LED .

\


<div align="left"><img src="https://desk.zoho.com/DocsDisplay?zgId=669162239&#x26;mode=inline&#x26;blockId=bbr0jdd48239ca2584474bf3d0721ab520983" alt=""></div>

Once the camera is powered, both the green and red LED of the Power indicator will be on.  The status indicator LED uses both green and red LED to indicate the current state of the system, per the following diagrams.

<div align="left"><img src="https://desk.zoho.com/DocsDisplay?zgId=669162239&#x26;mode=inline&#x26;blockId=bbr0j974eec1278984605982155e1ae847a3f" alt=""></div>

| <p>Initialization<br><em>Operation :</em>  The camera is initializing its components and performing startup functions.<br><br><em>State Time :</em>  Camera initialization can take up to 60 seconds.<br><br><em>Transition</em> : The camera transitions to the idle state immediately after the initialization of all camera components is completed.<br><br><em>Status Indicator</em> :  Off or <mark style="color:red;">F</mark>l<mark style="color:red;">a</mark>s<mark style="color:red;">h</mark>i<mark style="color:red;">n</mark>g <mark style="color:red;">r</mark>e<mark style="color:red;">d</mark>.<br></p>                                                                                             |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>Idle<br><em>Operation</em> : The camera is waiting to start a session.  Criteria for starting a session are based on configuration setting – see section Operation Modes.<br><br><em>State Time</em> : The state occurs indefinitely until criteria are met for starting the session.<br><br><em>Transition</em> :  The camera transitions to the active state once a session is started.  Transitions from the idle to active state can take up to 20 seconds.<br><br><em>Status Indicator</em> :  <mark style="color:green;">Solid green.</mark><br></p>                                                                                                                                                        |
| <p>Active<br><em>Operation</em> : The camera is able to take pictures and log these pictures along with metadata to the SD card. This state cannot be entered if the SDcard is missing or corrupt.<br><br><em>State Time</em> :  This state occurs indefinitely until criteria are met for closing the session.<br><br><em>Transition</em> : Transition to the idle state occurs if the session is closed.<br><br><em>Status Indicator</em> :  <mark style="color:green;">F</mark>l<mark style="color:green;">a</mark>s<mark style="color:green;">h</mark>i<mark style="color:green;">n</mark>g <mark style="color:green;">g</mark>r<mark style="color:green;">e</mark>e<mark style="color:green;">n</mark>.<br></p> |

\
