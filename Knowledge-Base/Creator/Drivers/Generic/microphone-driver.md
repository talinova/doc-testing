---
title: "Microphone Drivers"
tags: creator, driver, equipment, microphone, generic
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: This is a custom built-in driver that can adjust settings for any microphone.
---

# Microphone Drivers

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/microphone.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/microphone.png" alt="SAVI Creator Mic configuration" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Has Discrete Volume:** If enabled, this audio zone has discrete audio capability.

* **Default Volume:** For discrete zones, this is the volume level sent to the device when it is turned on.

* **Volume Preset (1-10):** Volume level for # in preset names list.

* **Alternate Volume Control:** Device Port used when sending volume related commands (setVolume, volumeUp, volumeDown, mute). This is only needed when the port connected to the microphone can not handle volume control.

### Connections

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/microphone-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/microphone-connections-output.png" alt="SAVI Creator Mic output connections" width="300" height="">
</a>

* **Output (1-5):** Connects to the Input of the audio device used for routing (such as the SAVI DSP).
