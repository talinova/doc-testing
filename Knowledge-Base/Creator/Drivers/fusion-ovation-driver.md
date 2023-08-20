---
title: "Ovation Music Player Driver"
tags: creator, driver, equipment, ovation, fusion, audio
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: Resource for the Ovation music server drivers.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/fusion-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/fusion-logo.png" alt="Fusion Research Logo" width="700" height="" class="center">
</a>
</div>

# Ovation Music Player Driver
This driver is compatible with both the [Solo](https://www.fusionrd.com/solo-2-source-music-server) and [Duet](https://www.fusionrd.com/duet-3-source-music-server) models.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ovation-music-player.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ovation-music-player.png" alt="Ovation music player configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **MAC Address:** The unique address of the device.

### Connections

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/ovation-music-player-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/ovation-music-player-connections-output.png" alt="Ovation music player output connections" width="300" height="">
</a>

* **Output:** Connects to the Input of the audio device used for routing (such as the SAVI DSP).

# Logitech Media Server
Ovation Music Player uses Logitech Media Server. To find the MAC address for the Creator driver, navigate to `http://[ip of player]:9000/settings/index.html` to the Information tab. All zones will be listed under Player Information which displays the Player MAC Address.

Be sure to use the IP address of the Ovation device that you navigated to and ***not*** the Player IP Address listed under Player Information.

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/logitech-media-server-information.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/logitech-media-server-information.png" alt="Logitech Media Server Information" width="600" height="">
</a>