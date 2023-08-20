---
title: "SAVI Connect I/O Drivers"
tags: creator, driver, equipment, savi, connect, ir, serial, rs232, relay
date:
  created: "03/29/2022"
  modified: "12/12/2022"
description: Resource for the SAVI Connect I/O drivers. Configuration for the IR, RS232, and Relay modules.
---

<div style="text-align: center">

<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/Logos/savi-04-blue.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/Logos/savi-04-blue.png" alt="SAVI Logo" width="700" height="">
</a>
</div>

# SAVI Connect I/O Drivers

The SAVI Connect I/O driver interface with SAVI's Connect I/O hardware in order to add legacy devices to the SAVI 3 system. In conjunction, these allow control of IR, RS-232, and Relay devices. Step-by-step instructions can be found [here](/Knowledge-Base/Creator/Drivers/SAVI/creating-ir-rs232-drivers.md "SAVI Connect I/O Drivers page").

## IR Module

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-ir-module.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-ir-module.png" alt="SAVI Connect IO IR Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Timeout (MSec):** The amount of time in milliseconds to wait for the connect, send and response before aborting. Set to 3000 as default.

* **Delay After Success (MSec):** The amount of time in milliseconds to wait after a successful command before sending another. Set to 1000 as default.

* **Delay After Failure (MSec):** The amount of time in milliseconds to wait after a failed command before sending another. Set to 1000 as default.

* **Configuration of port (1-3):** These set the IR ports to either Emitter or Sensor.
  * Emitter - Creates and projects IR signals (output).
  * Sensor - Reads contact signals (input). This requires a GCSC1 Sensor Contact Closure be plugged into the same port on the physical Connect I/O. Corresponds to the "sensor" setting from the web configuration page, not "sensor notify."

### Connections

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-ir-module-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-ir-module-connections-output.png" alt="SAVI Connect IO IR Module config" width="300" height="">
</a>

* **IR Out (1-3):** Connects to any IR endpoint or receiver.

## RS-232 Module

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-rs232-module.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-rs232-module.png" alt="SAVI Connect IO RS232 Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

### Connections

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-rs232-module-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-rs232-module-connections-output.png" alt="SAVI Connect IO RS232 Module config" width="300" height="">
</a>

* **RS232 Out 1:** Connects to any RS232 endpoint or receiver.



## Relay Module

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-relay-module.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-relay-module.png" alt="SAVI Connect IO Relay Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

### Connections

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-relay-module-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/savi-connect-io-relay-module-connections-output.png" alt="SAVI Connect IO Relay Module config" width="300" height="">
</a>

* **Relay Port (1-6):** Connects to relay modules.
