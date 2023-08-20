---
title: "VLC Controller Drivers"
tags: creator, driver, equipment, vlc, controller
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: Resource for the VLC Controller Driver for streaming VLC content.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/vlc-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/vlc-logo.png" alt="VLC Logo" width="700" height="">
</a>
</div>

# VLC Controller Drivers

This driver is used when running [VLC media player](https://www.videolan.org/vlc/) as a streaming server on a PC. The PC running VLC must be on the same network as SAVI.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/vlc-controller.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/vlc-controller.png" alt="Technicolor COM51 Tuner 01" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 8080 by default.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Name and URI pairs of playlists:** Format will be `[name], [uri]` without brackets and with a new line for each. URIs are case sensitive and can reference a file path of a playlist (with .xspf extension), a audio or video file, or even a network stream.
    >***URIs will create a list of playlists that can be controlled via macros.***
