---
title: "Generic TCP Driver"
tags: creator, driver, equipment, generic, telnet, tcp
date:
  created: "05/09/2022"
  modified: "12/12/2022"
description: This is a built-in driver that can connect to any telnet device for listing in Facility View.
---

# Generic TCP Driver
This driver is for devices which have instructions to control them over telnet but are not yet supported by SAVI directly. Unlike the [AV Switches Driver](av-switches-driver.md), this driver may be used for any device.

#### Properties
<a href="../../../../Assets/Knowledge-Base/Creator/Drivers/generic-telnet-device.png">
  <img src="../../../../Assets/Knowledge-Base/Creator/Drivers/generic-telnet-device.png" alt="generic Telnet device configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 23 by default.

* **User Prompt:** The prompt the systems sends to ask for a user name.

* **Username:** Login username of the device.

* **Password Prompt:** The prompt the systems sends to ask for a password.

* **Password:** Login password of the device.

* **Success Prompt:** The message displayed once a user has successfully connected and logged in.

* **Throttle delay (ms):** Controls the rate at which messages are sent to the device. (In milliseconds) Some devices may have a minimum delay requirement.
