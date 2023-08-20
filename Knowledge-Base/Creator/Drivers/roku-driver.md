---
title: "Roku Driver"
tags: creator, driver, equipment, roku
date:
  created: "05/13/2022"
  modified: "09/13/2022"
description: Resource for the Roku driver.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/roku-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/roku-logo.png" alt="Roku Logo" width="700" height="">
</a>
</div>

# Roku Driver
This driver is used as a satellite source for connecting to a [Roku](https://www.roku.com/) device.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/roku.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/roku.png" alt="Roku configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Image Preview URL:** A link used to preview a streaming video source. If the driver is connected to a Stream.One, this field will auto-populate. This provides the appropriate URL to SAVI Preview in Facility View. Allowable: single image preview or Motion JPEG.
* **Image Preview Refresh Interval:** Determines how often the preview image should be refreshed.
    * If Image Preview URL refers to single image preview, specifies Refresh Interval in Milliseconds (default is 67 which is equal to 15 frames per second).
    * If Image preview URL refers to Motion JPEG, set to 0.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 8060 by default.

* **Serial Number:** The serial number of the specific device.
