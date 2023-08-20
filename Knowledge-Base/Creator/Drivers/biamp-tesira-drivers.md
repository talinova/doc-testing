---
title: "Biamp Tesira Drivers"
tags: creator, driver, equipment, biamp, tesira
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: IP drivers for Biamp Tesira devices.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/biamp-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/biamp-logo.png" alt="Biamp Logo" width="700" height="" class="center">
</a>
</div>

# Biamp Tesira Drivers

These drivers directly interact with the [Biamp Tesira line](https://www.biamp.com/products/product-families/tesira) of hardware and configured software to control source selection and volume control with SAVI. There are four separate drivers for this device, but not all are utilized at the same time. One driver is needed for volume control and another for source selection.

### Tesira Level
The level driver controls minimum and maximum volume range as well as how the volume scale is displayed.

You will also need to set this driver as the **Alternate Volume Control** in the **Audio Zone** driver.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-level.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-level.png" alt="Biamp Tesira Level configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Instance Tag:** The Instance ID/Device ID of the processing block.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Volume Scale:** How the volume is displayed.
  * dB - In decibels.
  * Percentage - 0 to 100 percent.

* **Max dB:** Maximum decibels allowed. Set to 12 by default.

* **Min dB:** Minimum decibels allowed. Set to -100 by default.

* **Mute Type:** Select how mute functions.
  * Mute - Completely mutes the audio channel.
  * Level - Utilizes the **Mute Level** to set an audio channel to a specific volume.

* **Mute Level:** What to set volume to when muting by level. Set to -100 by default.

### Connections
If using this driver as an Alternate Volume Control, leave all connections blank.

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-level-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-level-connections-input.png" alt="Biamp Tesira Level - connections - input" width="300" height="">
</a>

* **Input (1-36):** Supports up to thirty-six audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-level-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-level-connections-output.png" alt="Biamp Tesira Level - connections - output" width="300" height="">
</a>

* **Output (1-36):** Supports up to thirty-six audio outputs depending on device. Is still limited by the logical ports within the biamp system.


------------

## Source Selection

The Matrix Mixer, Router Block, and Source Selector are different drivers that each complete roughly the same function. The driver you use is determined by the biamp UI configuration. Choose **one** of these drivers to complete your source selection within SAVI.

### Tesira Matrix Mixer
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-01.png" alt="Biamp Tesira Matrix Mixer 01 configuration" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-02.png" alt="Biamp Tesira Matrix Mixer 02 configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Instance Tag:** The Instance ID/Device ID of the processing block. Created within the biamp software.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Use Crosspoint Levels:** Determines if volume can be adjusted at the crosspoint.
  * Yes - Enable crosspoint levels.
  * No - Disable crosspoint levels.

* **Volume Scale:** How the volume is displayed.
  * dB - In decibels.
  * Percentage - 0 to 100 percent.

* **Output (1-36) Max dB:** Maximum decibels allowed. Set to 12 by default.

* **Output (1-36) Min dB:** Minimum decibels allowed. Set to -100 by default.

* **Mute Type:** Select how mute functions.
  * Mute - Completely mutes the audio channel.
  * Level - Utilizes the **Mute Level** to set an audio channel to a specific volume.

* **Mute Level:** What to set volume to when muting by level. Set to -100 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-connections-input.png" alt="Biamp Tesira Matrix Mixer - connections - input" width="300" height="">
</a>

* **Input (1-36):** Supports up to thirty-six audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-matrix-mixer-connections-output.png" alt="Biamp Tesira Matrix Mixer - connections - output" width="300" height="">
</a>


* **Output (1-36):** Supports up to thirty-six audio outputs depending on device. Is still limited by the logical ports within the biamp system.















### Tesira Router Block
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-router-block.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-router-block.png" alt="Biamp Tesira Router Block configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Instance Tag:** The Instance ID/Device ID of the processing block. Created within the biamp software.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-router-block-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-router-block-connections-input.png" alt="Biamp Tesira Router Block - connections - input" width="300" height="">
</a>

* **Input (1-50):** Supports up to fifty audio inputs depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-router-block-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-router-block-connections-output.png" alt="Biamp Tesira Router Block - connections - output" width="300" height="">
</a>

* **Output (1-50):** Supports up to fifty audio outputs depending on device. Is still limited by the logical ports within the biamp system.















### Tesira Source Selector
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-01.png" alt="Biamp Tesira Source Selector 01 configuration" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-02.png" alt="Biamp Tesira Source Selector 02 configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Instance Tag:** The Instance ID/Device ID of the processing block. Created within the biamp software.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Volume Scale:** How the volume is displayed.
  * dB - In decibels.
  * Percentage - 0 to 100 percent.

* **Output Max dB:** Maximum decibels allowed. Set to 12 by default.

* **Output Min dB:** Minimum decibels allowed. Set to -100 by default.

* **Source (1-32) Max dB:** Maximum decibels allowed. Set to 12 by default.

* **Source (1-32) Min dB:** Minimum decibels allowed. Set to -100 by default.


#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-connections-input.png" alt="Biamp Tesira Source Selector - connections - input" width="300" height="">
</a>

* **Input (1-36):** Supports up to thrity-six audio inputs, depending on device. Is still limited by the logical ports within the biamp system.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/biamp-tesira-source-selector-connections-output.png" alt="Biamp Tesira Source Selector - connections - output" width="300" height="">
</a>

* **Output:** Connects to the Audio Zone associated with the Sourse Selector device.
