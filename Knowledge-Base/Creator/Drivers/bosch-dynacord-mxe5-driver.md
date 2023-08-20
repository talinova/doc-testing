---
title: "Bosch Dynacord MXE5 Driver"
tags: creator, driver, equipment, bosch, dynacord, mxe5, dsp
date:
  created: "09/29/2022"
  modified: "10/31/2022"
description: IP driver for the Bosch Dynacord MXE5 device.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/bosch-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/bosch-logo.png" alt="Bosch Logo" width="700" height="">
</a>
</div>

# Bosch Dynacord MXE5 Driver
This driver allows control over source selection and volume on the [MXE5 Matrix mix engine](https://products.dynacord.com/na/en/mxe5/) through the Sonicue software. This driver represents the virtual mixer within that software and is connected to only one output. Add a new Zone Mixer driver for each output.


#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/bosch-dynacord-mxe5-dsp-zone-mixer.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/bosch-dynacord-mxe5-dsp-zone-mixer.png" alt="Bosch Dynacord MXE5 configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Zone ID:** This refers to the setting of the same name within the Sonicue software.

* **Minimum decibel range:** Minimum decibels allowed. Set to -80 by default.

* **Maximum decibel range:** Maximum decibels allowed. Set to 10 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/bosch-dynacord-mxe5-dsp-zone-mixer-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/bosch-dynacord-mxe5-dsp-zone-mixer-connections-input.png" alt="Bosch Dynacord MXE5 input connections" width="230" height="">
</a>

* **Input (01-24):** Up to twenty-four audio inputs included in this mix.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/bosch-dynacord-mxe5-dsp-zone-mixer-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/bosch-dynacord-mxe5-dsp-zone-mixer-connections-output.png" alt="Bosch Dynacord MXE5 output connections" width="230" height="">
</a>


* **Output 01:** One of the audio outputs.
