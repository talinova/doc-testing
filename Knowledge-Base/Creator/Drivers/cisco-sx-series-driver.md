---
title: "Cisco SX Series Driver"
tags: creator, driver, equipment, cisco, sx, conference, teleconference
date:
  created: "09/13/2022"
  modified: "12/12/2022"
description: Resource for the SX Series Cisco driver.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/cisco-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/cisco-logo.png" alt="Cisco Logo" width="700" height="" class="center">
</a>
</div>

# Cisco SX Series Driver


This driver interfaces with [Cisco's TelePresence SX Series](https://www.cisco.com/c/en/us/support/collaboration-endpoints/telepresence-quick-set-series/series.html) teleconferencing devices.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/cisco-sx-series.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/cisco-sx-series.png" alt="SAVI Creator Cisco SX series configuration" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Call Conferencing:** Enables support for Cisco codec "Add to Call" conferencing.

* **Call Holding:** Enables support for putting calls on hold.

* **Video Conferencing:** Enables support for camera controls.

* **On Screen Controls:** Enables support for displaying controls on the screen.

* **Camera Positions:** Enables support for Cisco saved camera positions.

* **Use SAVI Phonebook:** Enable/Disable SAVI UI for SAVI internal contact management. Synced contacts from the device cannot be edited/deleted from SAVI.

* **Phonebook Type:**
  * **None:** No phonebook.
  * **Local:** Phonebook is stored on the physical device.
  * **Corporate:** Retrieves phonebook information from the TMS server.

* **SAVI Volume Controls:** Determines how SAVI volume controls the Cisco device.
  * **Hide Volume Buttons:** Removes volume controls from the interface.
  * **Controls Device Volume:** Volume controls the device volume.
  * **Controls Room Volume:** Volume controls the room speaker volume.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/cisco-sx-series-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/cisco-sx-series-connections-input.png" alt="SAVI Creator Cisco SX series input connections" width="300" height="">
</a>

* **PC Audio:** Standard 3.5mm audio jack.

* **DVI:** Connection to video source.

* **Mic 1:** Primary MIC input.

* **Mic 2:** Secondary MIC input.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/cisco-sx-series-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/cisco-sx-series-connections-output.png" alt="SAVI Creator Cisco SX series output connections" width="300" height="">
</a>

* **Headphones:** Standard 3.5mm audio jack.

* **HDMI 1:** Primary audio/video output.

* **HDMI 2:** Secondary audio/video output.
