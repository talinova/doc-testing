---
title: "Spyder X20 Driver"
tags: creator, driver, macro, christie, spyder, internal
date:
  created: "05/19/2022"
  modified: "12/12/2022"
description: Resource for the Christie Spyder X20 Driver.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/christie-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/christie-logo.png" alt="christie Logo" width="700" height="">
</a>
</div>

# Spyder X20 Driver
This driver is unique in that it does not add a driver controller to Equipment or Connections. It instead creates a Macro for changing presets on the [device](https://www.christiedigital.com/products/image-processors/christie-spyder-x20/overview). The macro will still need to be configured under the Macros section of Creator.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/christie-spyder-x20-preset.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/christie-spyder-x20-preset.png" alt="Christie Spyder x20 Preset" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 11116 by default.

* **Preset ID:** The unique identifier of the preset you wish to control.

* **Duration:** Choose how long (in seconds) an image/video shows before transitioning to the next. Set to 60 by default.
