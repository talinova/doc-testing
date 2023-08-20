---
title: "Biamp AudiaFLEX Drivers"
tags: creator, driver, equipment, biamp, audiaflex
date:
  created: "05/12/2022"
  modified: "12/12/2022"
description: IP and serial (RS232) drivers for Biamp AudiaFLEX devices.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/biamp-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/biamp-logo.png" alt="Biamp Logo" width="700" height="" class="center">
</a>
</div>

# Biamp AudiaFLEX Drivers

These drivers directly interact with [biamp AudiaFLEX](https://support.biamp.com/Audia-Nexia) hardware to control source selection and volume control with SAVI. There are four separate drivers for this device, but not all are utilized at the same time. One driver is needed for volume control and another for source selection.

## IP Drivers
### IP Biamp AudiaFLEX Control
This driver is used for volume control.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control.png" alt="Biamp AudiaFLEX Control configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 23 by default.

* **Device Number:** Determines the position of the unit in a chain of up to 15. Set to 1 by default.

* **Instance ID:** The Device ID/Instance Tag of the processing block.

* **Minimum decibel range:** Minimum decibels allowed. Set to -100 by default.

* **Maximum decibel range:** Maximum decibels allowed. Set to 12 by default.

### Connections
If using this driver as an Alternate Volume Control, leave all connections blank.

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control-connections-input.png" alt="Biamp AudiaFLEX Control - connections ip - input" width="300" height="">
</a>

* **Input (1-50):** Supports up to fifty audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control-connections-output.png" alt="Biamp AudiaFLEX Control ip - connections - output" width="300" height="">
</a>

* **Output (1-50):** Supports up to fifty audio outputs depending on device. Is still limited by the logical ports within the biamp system.


### IP Biamp AudiaFLEX Router
This driver is used for source selection.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-router.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-router.png" alt="Biamp AudiaFLEX router ip configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 23 by default.

* **Device Number:** Determines the position of the unit in a chain of up to 15. Set to 1 by default.

* **Instance ID:** The Device ID/Instance Tag of the processing block.


### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-router-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-router-connections-input.png" alt="Biamp AudiaFLEX router ip - connections - input" width="300" height="">
</a>

* **Input (1-50):** Supports up to fifty audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-router-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-router-connections-output.png" alt="Biamp AudiaFLEX router ip - connections - output" width="300" height="">
</a>

* **Output (1-50):** Supports up to fifty audio outputs depending on device. Is still limited by the logical ports within the biamp system.

----

## Serial Drivers
### Serial Biamp AudiaFLEX Control
This driver is used for volume control.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-control.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-control.png" alt="Biamp AudiaFLEX Control Serial configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Baud Rate:** Set to 38400 by default.

* **Flow Control:** Sets the serial port handshake type.
  * None - Turned off.
  * Hardware - Hardware flow control.
  * XON/XOFF - Software flow control.
  * Unknown - Flow control is unknown.

* **Parity:** Sets the serial port parity type for error detection.
  * None - Turned off.
  * Even - Even parity bit.
  * Odd - Odd parity bit.
  * Unknown - Parity is unknown.

* **Data Bits:** Set to 8.

* **Stop Bits:** Set to either 1 or 2.

* **Device Number:** Determines the position of the unit in a chain of up to 15. Set to 1 by default.

* **Instance ID:** The Device ID/Instance Tag of the processing block.

* **Device Number:** Determines the position of the unit in a chain of up to 15. Set to 1 by default.

* **Instance ID:** The Device ID/Instance Tag of the processing block.

* **Minimum decibel range:** Minimum decibels allowed. Set to -100 by default.

* **Maximum decibel range:** Maximum decibels allowed. Set to 12 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-control-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-control-connections-input.png" alt="Biamp AudiaFLEX Control serial - connections - input" width="300" height="">
</a>

* **Input (1-50):** Supports up to fifty audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ip-biamp-audiaflex-control-connections-output.png" alt="Biamp AudiaFLEX Control serial - connections - output" width="300" height="">
</a>

* **Output (1-50):** Supports up to fifty audio outputs depending on device. Is still limited by the logical ports within the biamp system.


### Serial Biamp AudiaFLEX Router
This driver is used for source selection.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-router.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-router.png" alt="Biamp AudiaFLEX router serial configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Baud Rate:** Set to 38400 by default.

* **Flow Control:** Sets the serial port handshake type.
  * None - Turned off.
  * Hardware - Hardware flow control.
  * XON/XOFF - Software flow control.
  * Unknown - Flow control is unknown.

* **Parity:** Sets the serial port parity type for error detection.
  * None - Turned off.
  * Even - Even parity bit.
  * Odd - Odd parity bit.
  * Unknown - Parity is unknown.

* **Data Bits:** Set to 8.

* **Stop Bits:** Set to either 1 or 2.

* **Device Number:** Determines the position of the unit in a chain of up to 15. Set to 1 by default.

* **Instance ID:** The Device ID/Instance Tag of the processing block.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-router-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-router-connections-input.png" alt="Biamp AudiaFLEX router serial - connections - input" width="300" height="">
</a>

* **Input (1-50):** Supports up to fifty audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-router-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/serial-biamp-audiaflex-router-connections-output.png" alt="Biamp AudiaFLEX router serial - connections - output" width="300" height="">
</a>

* **Output (1-50):** Supports up to fifty audio outputs depending on device. Is still limited by the logical ports within the biamp system.
