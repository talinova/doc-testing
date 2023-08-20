---
title: "Zektor ProAudio 32 Driver"
tags: creator, driver, equipment, zektor
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: Resource for the Lutron ProAudio 32 driver.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/zektor.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/zektor.png" alt="Zektor Logo" width="700" height="">
</a>
</div>

# Zektor ProAudio 32 Driver
This driver interfaces with this specific [Zektor audio matrix](https://www.pulse-eight.com/p/212/proaudio-32 "Zektor audio matrix"). Specifications on the matrix itself can be found on the Pulse Eight site.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-01.png" alt="Zektor PROAUDIO32 01" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-02.png" alt="Zektor PROAUDIO32 02" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-03.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-03.png" alt="Zektor PROAUDIO32 03" width="230" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 50005 by default.

* **Has Discrete Volume:** This is always enabled.

* **Analog Input (01-80) Audio Gain:** The number corresponds to dB. Set to 0 by default.

* **Analog Input (01-80) Audio Delay:** Introduces an audio delay in milliseconds. Set to 0 by default.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-input-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-input-01.png" alt="Zektor PROAUDIO32 - connections - input 01" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-input-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-input-02.png" alt="Zektor PROAUDIO32 - connections - input 02" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-input-03.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-input-03.png" alt="Zektor PROAUDIO32 - connections - input 03" width="230" height="">
</a>

* **Analog Input (01-32):** L/R audio source.

* **Coax Input (33-64):** Digital coaxial source.

* **Optical Input (65-80):** Digital optical source.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-output-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-output-01.png" alt="Zektor PROAUDIO32 - connections - output 01" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-output-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio32-connections-output-02.png" alt="Zektor PROAUDIO32 - connections - output 02" width="230" height="">
</a>

* **Analog Output (01-32):** Digital coaxial output.

* **Coax Output (01-32):** Digital optical output.
