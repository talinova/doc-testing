---
title: "RGBLink X3 Driver"
tags: creator, driver, equipment, rgblink
date:
  created: "03/25/2022"
  modified: "09/13/2022"
description: Resource for the RGBLink X3 Video Wall driver.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/rgblink-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/rgblink-logo.png" alt="RGBLink Logo" width="700" height="">
</a>
</div>

# RGBLink X3 Video Wall Drivers
This driver is specifically designed for the [X3 Video Wall](https://www.rgblink.com/productsinfo.aspx?id=73) device. It is meant to be used in conjunction with a [Video Wall Zone Placeholder](/Knowledge-Base/Creator/Drivers/Generic/video-wall-zone-driver.md). A Video Wall Zone driver should be used for each source layout in the RGBLink UI.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall.png" alt="RGBLink X3 Video Wall" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-connections-input.png" alt="RGBLink X3 Video Wall - connections input" width="300" height="">
</a>


* **Input (01-16):** Up to sixteen sources.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-connections-output.png" alt="RGBLink X3 Video Wall - connections - output" width="300" height="">
</a>


* **Output (01-16):** Up to sixteen outputs. Each output should be connected to an X3 Video Wall Zone driver.






<!--
## X3 Video Wall Zone
One of these drivers are needed for each layout in the RGB UI. Be sure to import your RGB project file into SAVI through the `/admin` page.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-zone.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-zone.png" alt="RGBLink X3 Video Wall zone" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Hidden Sources:** The destination IP address that SAVI will use when communicating with the device.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-zone-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rgblink-x3-video-wall-zone-connections-input.png" alt="RGBLink X3 Video Wall zone - connections - input" width="300" height="">
</a>

* **HDMI:** HDMI source input.
-->
