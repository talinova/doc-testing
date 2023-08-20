---
title: "Generic Source Driver"
tags: creator, driver, equipment, generic
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: This is a built-in driver that can connect to any source for listing in Facility View.
---

# Generic Source Driver

The Generic Source driver allows adding non-controllable sources to the system. From gaming systems to basic stereos, computer displays to undefined HDMI inputs, connect any device that doesn't have a specific driver and cannot accept commands.

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/generic-source.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/generic-source.png" alt="generic source configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Image Preview URL:** The URL to an image that SAVI will display in the “Remote Modal”. For Stream.One connected devices, this would show a live image preview containing the output from the device.

* **Image Preview Refresh Interval:** If you use the Image Preview, then this will set how often SAVI should refresh (reload) that image. If you chose a motion jpeg as the Image Preview, set this to 0.

### Connections

##### Output
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/generic-source-connections-output.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/generic-source-connections-output.png" alt="generic source output connections" width="300" height="">
</a>

* **Output:** Any input device.
