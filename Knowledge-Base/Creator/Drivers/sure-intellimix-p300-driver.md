---
title: "Shure Intellimix P300 Driver"
tags: creator, driver, equipment, shure
date:
  created: "05/13/2022"
  modified: "09/13/2022"
description: Resource for the Shure Intellimix P300 drivers.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/shure-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/shure-logo.png" alt="Shure Logo" width="700" height="" class="center">
</a>
</div>

# Shure Intellimix P300 Driver
This driver interfaces with this specific [Shure  audio conferencing processor](https://www.shure.com/en-US/products/mixers/p300 "Atlona video matrix"). Specifications on the device can be found on the Shure site.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/shure-intellimix-p300.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/shure-intellimix-p300.png" alt="Shure Intellimix P300 configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 2202 by default.

* **Command Throttle:** Specifies the number of milliseconds to wait between sending commands. Set to 50 by default.

### Connections
Most inputs and outputs are assignable in the Receiver settings of the Shure UI. Setup will include choosing which physical connections are being used for each of the assignable inputs or outputs.



##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/shure-intellimix-p300-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/shure-intellimix-p300-connections-input.png" alt="Shure Intellimix P300 - input" width="300" height="">
</a>


* **All:** Used if a source is available to all inputs.

* **Dante Input Channel (1-10):** Digital inputs through ethernet network with Dante.

* **Analog Input Channel (1-2):** Euroblock inputs.

* **USB Input Channel 1:** USB port access. May be used for either input or output.

* **Mobile Input Channel 1:** Standard 3.5mm audio jack.

* **Automixer:** Devices which should be routed through the Shure UI Automixer.


##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/shure-intellimix-p300-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/shure-intellimix-p300-connections-output.png" alt="Shure Intellimix P300 - output" width="300" height="">
</a>

* **Dante Output Channel (1-8):** Digital outputs through ethernet network.

* **Analog Output Channel (1-2):** Euroblock outputs.

* **USB Output Channel 1:** USB port access. May be used for either input or output.

* **Mobile Output Channel 1:** Standard 3.5mm audio jack.
