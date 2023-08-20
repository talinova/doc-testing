---
title: "Technicolor COM51 Driver"
tags: creator, driver, equipment, technicolor, com51, com3000
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: Resource for the Technicolor COM51 drivers to control the COM3000 system.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/technicolor-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/technicolor-logo.png" alt="Technicolor Logo" width="700" height="">
</a>
</div>

# Technicolor COM51 Driver

Part of the [Technicolor COM3000](https://www.technicolor.com/connect/commercial-video-solutions/com3000-solution) configuration. This driver enables UI and macro control as well as settings configuration for a single COM51 tuner slot. Additionally, it provides Pro:Idiom configuration, canvas content control, and remote key controls through the SAVI UI.

One driver will be needed for ***each*** tuner configured in each COM51 card. By default, COM51s have 8 licensed tuners each, but you may purchase additional licenses (up to 23 per card) from Technicolor.

For a detailed walkthrough, check out our [setup guide](/Documentation/COM3000-Setup-Guide.pdf)

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/technicolor-com51-tuner.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/technicolor-com51-tuner.png" alt="Technicolor COM51 Tuner" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Image Preview URL:** Specify a jpeg or motion jpeg url that contains an image preview for this device.

* **Image Preview Refresh Interval:** If greater than 0, the Image Preview is automatically reloaded at this frequency (in msec). Set to 67 by default.

* **Management IP:** The IP address at which the COM3000's management page can be found.

* **Chassis:** Chassis number from COM3000 Overview page.

* **Slot:** Slot number from COM3000 Overview page.

* **Tuner:** Tuner number from COM3000 Overview page.

* **URL:** The URL of the multicast channel (i.e. rtp://234.1.100.1:5004). Will be automatically filled.

* **Pro:Idiom Encrypted:** Enable this if the Tuner uses LG's Pro:Idiom encryption technology. Will be automatically filled.
