---
title: "SAVI Canvas Encoder Driver"
tags: creator, driver, equipment, savi, canvas, encoder
date:
  created: "03/29/2022"
  modified: "12/12/2022"
description: Resource for the SAVI thermostat driver.
---

<div style="text-align: center">

<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/Logos/savi-canvas-color-dark.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/Logos/savi-canvas-color-dark.png" alt="SAVI Logo" width="700" height="">
</a>
</div>

# SAVI Canvas Encoder Driver
This driver is usable with any device that supplies a compatible stream. It allows attaching a stream to a source so it appears in the Source list in Facility View.

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/canvas-encoder.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/canvas-encoder.png" alt="SAVI Canvas Encoder - configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Stream URL:** The base URL for this encoder (i.e. `rtp://239.1.1.1:5006`).

### Connections

##### Input
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/canvas-encoder-connections-input.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/canvas-encoder-connections-input.png" alt="SAVI Canvas Encoder - connections- inputs" width="300" height="">
</a>

* **Input:** Connects to a video source.
