---
title: "Samsung Drivers"
tags: creator, driver, equipment, samsung
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: Resource for the Samsung drivers.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/samsung-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/samsung-logo.png" alt="Samsung Logo" width="700" height="">
</a>
</div>

# Samsung Drivers
These drivers support the [OHF](https://displaysolutions.samsung.com/digital-signage/detail/1050/OH55F) and [BHT](https://displaysolutions.samsung.com/digital-signage/detail/1647/BH75T) lines of IP controlled displays. You may need to enable "Allow IP remote" in the display settings.

>**When adding these devices to the project, the display will receive a popup from the SAVI App to allow or deny connection. Allow this connection in order to connect to SAVI. Denying this request will require adding the connection manually in the display's menu.**

## Signage OHF
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-signage-ohf.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-signage-ohf.png" alt="Samsung Signage OHF" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Hidden Sources:** Sources that should not be shown when selecting sources for this device.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Default Volume:** This is the volume level sent to the device when it is turned on.

* **Power On Interval:** The number of milliseconds to wait after sending ON. Set to 60000 (1 min) by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-signage-ohf-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-signage-ohf-connections-input.png" alt="Samsung Signage OHF - connections - input" width="300" height="">
</a>

* **HDBT:** HDBaseT ethernet source.

* **HDMI (1-2):** Up to two HDMI sources.


----------------


## TV BHT
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-tv-bht.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-tv-bht.png" alt="Samsung TV BHT" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Hidden Sources:** The sources that should not be shown when selecting sources for this device.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **MAC Address:** Media Access Control Address (read only).

* **Access Token:** Used to identify SAVI with the TV (read only).

* **Power On Interval:** The number of milliseconds to wait after sending ON. Set to 5000 (5 sec) by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-tv-bht-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/samsung-tv-bht-connections-input.png" alt="Samsung TV BHT - connections - input" width="300" height="">
</a>

* **HDMI:** HDMI source.
