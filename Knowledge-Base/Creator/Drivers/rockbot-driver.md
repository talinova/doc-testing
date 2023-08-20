---
title: "Rockbot Driver"
tags: creator, driver, equipment, rockbot, audio
date:
  created: "03/28/2022"
  modified: "12/12/2022"
description: Resource for the Rockbot music server drivers.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/rockbot-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/rockbot-logo.png" alt="Rockbot Logo" width="700" height="">
</a>
</div>

# Rockbot Driver
This driver provides interface control through SAVI for interacting with [Rockbot Music service](https://rockbot.com/). Provides access to artist and playlist searching, play/skip controls, and thumbs up/down feedback to Rockbot.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rockbot-music-player.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rockbot-music-player.png" alt="Rockbot music player configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **API Key:** The API Key for this device, obtained from Rockbot.
  >Contact Christopher Ezell at chris@rockbot.com to obtain your API Key.

### Connections

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/rockbot-music-player-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/rockbot-music-player-connections-output.png" alt="Rockbot music player output connections" width="300" height="">
</a>

* **Output:** Connects to the Input of the audio device used for routing (such as the SAVI DSP).
