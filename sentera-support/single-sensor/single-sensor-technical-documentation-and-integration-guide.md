# Single Sensor Technical Documentation & Integration Guide

**Resources**

Scroll to the bottom of the page to download the _Using Sentera Sensors with MAVLink and Pixhawk_ document, as well as download these documents below for technical details on the Sentera Singles Sensor and instructions for integrating with other systems:

* [Sentera Single Hardware Integration Guide (.pdf)](https://drive.google.com/file/d/1da9d1Y4IMC1tieSy7Jh4bQHCLuGc5RI5/view?usp=sharing)
* [Sentera Single Cad Model (.step)](https://docs.zohopublic.com/file/bkfhu7089a0a69b634790a5430054f7c97c27)
* [Sentera Single Interface Control Drawing (.pdf](https://drive.google.com/file/d/0B92nAKa94wI7WjZaWmpiM3BnZHM/view?usp=sharing))

**Sentera Single Hardware Integration**

You can easily integrate the Sentera Single Sensor with a wide range of systems. These include interfaces to power the camera, as well as external devices that can be powered by the camera. Supported devices include:&#x20;

* Lockheed Martin Kestrel autopilot (3.3V UART)
* Pixhawk autopilot (3.3V UART)
* MAVLink based systems (3.3V UART)
* Sentera based systems (100Base-T Ethernet)
* GPS based triggering/metadata (PWR and 3.3V UART)
* Sentera Light Sensor (3.3V I2C)
* Customized ICD options available upon request

You can purchase camera cable interfaces directly from Sentera. Major suppliers also offer pre-terminated cables/contracts that allow you to create cable installations to suit your specific requirements. \
\
J1 - Ethernet&#x20;

Connector J1 is a 100Base-T Ethernet interface that can be used for all camera functions as detailed below. Most standard interfaces do not require the Ethernet interface. You can also use the J1-Ethernet interface to access the camera's microSD card when the device is on the ground.

| Pin | Signal | Type | T568A Color |
| --- | ------ | ---- | ----------- |
| 1   | TX+    | I/O  | GRN/WHT     |
| 2   | TX-    | I/O  | GRN         |
| 3   | RX+    | I/O  | ORG/WHT     |
| 4   | RX-    | I/O  | ORG         |

Connector: 53047-0410

Mating Connector: 51021-0400

\
J2 - Power and I/O

Connector J2 is a Power and I/O connector. It typically is used to help trigger the camera from the flight controller of GPS receiver. It provides a 3.3V voltage source to power the Sentera Light Sensor and/or an external GPS receiver. \


| Pin          | Signal              | Type           | Description                                      |
| ------------ | ------------------- | -------------- | ------------------------------------------------ |
| <p>1<br></p> | <p>VBATT<br></p>    | <p>PWR<br></p> | <p>6 to 26V Input - 2.4W @ 12VIn typical<br></p> |
| <p>2<br></p> | <p>GND<br></p>      | <p>PWR<br></p> | <p><br></p>                                      |
| <p>3<br></p> | <p>(3V3)RXD<br></p> | <p>I<br></p>   | <p>3.3V UART Input<br></p>                       |
| <p>4<br></p> | <p>(3V3)TXD<br></p> | <p>O<br></p>   | <p>3.3V UART Output<br></p>                      |
| <p>5<br></p> | <p>VCC_3V3<br></p>  | <p>PWR<br></p> | <p>3.3VDC @ 1A. Power Output<br></p>             |
| <p>6<br></p> | <p>GND<br></p>      | <p>PWR<br></p> | <p><br></p>                                      |
| <p>7<br></p> | <p>(3V3)SCL<br></p> | <p>I/O<br></p> | <p>3.3V I2C - Light Sensor<br></p>               |
| <p>8<br></p> | <p>V)SDA<br></p>    | <p>I/O<br></p> | <p>3.3V I2C - Light Sensor<br></p>               |

Connector: 53047-0810

Mating Connector: 51021-0800
