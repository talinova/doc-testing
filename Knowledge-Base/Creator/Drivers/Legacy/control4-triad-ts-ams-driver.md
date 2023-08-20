---
title: "Legacy Triad TS-AMS Audio Matrix Driver"
tags: creator, driver, internal, equipment, control4, ts-ams24, legacy
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: Resource for legacy Control4 drivers available only on select existing projects.
---
<div style="text-align: center">

<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/Logos/control-4-logo.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/Logos/control-4-logo.png" alt="Control4 Logo" width="" height="" class="center">
</a>
</div>

# Legacy Triad TS-AMS Audio Matrix Driver
This driver interfaces with this specific [Control4 power amplifier](https://www.control4.com/solutions/products/amplifiers-and-receivers/ "Control4 power amplifier"). Specifications on the matrix itself can be found on the Control4 site.

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24.png" alt="Control4 Audio Matrix Triad TS-AMS24" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The network port used for the IP address. Set to 52000 by default.

* **Throttle time (ms):** This device may have issues processing too many commands at once. This value will be how many milliseconds to wait after each command to the unit. Set to 500 by default.

* **TS-AMS model:** Select if you are using the 8 or 24 model switch.

### Connections

##### Input
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24-connections-input-01.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24-connections-input-01.png" alt="Control4 Audio Matrix Triad TS-AMS24 - connections - input 01" width="300" height="">
</a>
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24-connections-input-02.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24-connections-input-02.png" alt="Control4 Audio Matrix Triad TS-AMS24 - connections - input 02" width="300" height="">
</a>

* **Analog Input (01-16):** Up to sixteen L/R audio sources.
  >***Note: When using the 8x8 model, only use the first 8 Analog Inputs.***

* **Digital Input (17-24):** Up to eight digital audio sources (coaxial or optical - 17-24 corresponds to 9-16 on the rear of the device).
  >***Note: When using the 8x8 model, only use the first 4 Digital Inputs (17-21 corresponds to 5-8 on the rear of the device).***

>***Note: Analog inputs 9-16 and digital inputs 17-24 overlap.***

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/control4-audio-matrix-triad-ts-ams24-connections-output.png" alt="Control4 Audio Matrix Triad TS-AMS24 - connections - output" width="300" height="">
</a>

* **Analog Output (01-24):** Up to sixteen L/R audio outputs.
  >***Note: When using the 8x8 model, only the first 8 outputs are accessable.***

