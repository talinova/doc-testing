---
title: "RF Modulator Driver"
tags: creator, driver, equipment, rf, modulator, generic
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: This is a custom built-in driver that can adjust settings for any RF modulator.
---

# RF Modulator Driver

RF Modulators convert audio/video sources into coaxial RF signals which can then be connected to displays (such as the Sunbrite IP TV). These do not work with canvas displays as those are not equipped with tuner inputs. This driver is uncontrollable in SAVI.

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-01.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-01.png" alt="RF Modulator 02" width="300" height="">
</a>
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-02.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-02.png" alt="RF Modulator 02" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Input (01-36) Channel:** Assign channel numbers/names. These should match channels available from the inputs.

### Connections

##### Input
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-connections-input.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-connections-input.png" alt="RF Modulator - connections input" width="300" height="">
</a>


* **Input (1-36):** Up to thirty-six sources. Each source should match the device physically connected to the RF Modulator.

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/rf-modulator-connections-output.png" alt="RF Modulator - connections - output" width="300" height="">
</a>

* **Output:** RF output. This should be a display with a tuner input.
