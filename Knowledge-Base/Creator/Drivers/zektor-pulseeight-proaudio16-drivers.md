---
title: "Zektor ProAudio 16 Driver"
tags: creator, driver, equipment, zektor
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: Resource for the Lutron ProAudio 16 driver.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/zektor.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/zektor.png" alt="Zektor Logo" width="700" height="">
</a>
</div>

# Zektor ProAudio 16 Driver
This driver interfaces with this specific [Zektor audio matrix](https://www.pulse-eight.com/p/210/proaudio-16 "Zektor audio matrix"). Specifications on the matrix itself can be found on the Pulse Eight site.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-01.png" alt="Zektor PROAUDIO16 01" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-02.png" alt="Zektor PROAUDIO16 02" width="230" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 50005 by default.

* **Has Discrete Volume:** This is always enabled.

* **Analog Input (01-48) Audio Gain:** The number corresponds to dB. Set to 0 by default.

* **Analog Input (01-48) Audio Delay:** Introduces an audio delay in milliseconds. Set to 0 by default.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-input-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-input-01.png" alt="Zektor PROAUDIO16 - connections - input 01" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-input-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-input-02.png" alt="Zektor PROAUDIO16 - connections - input 02" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-input-03.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-input-03.png" alt="Zektor PROAUDIO16 - connections - input 03" width="230" height="">
</a>

* **Analog Input (01-16):** L/R audio source.

* **Coax Input (17-32):** Digital coaxial source.

* **Optical Input (33-48):** Digital optical source.


##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-output-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-output-01.png" alt="Zektor PROAUDIO16 - connections - output 01" width="230" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-output-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/zektor-proaudio16-connections-output-02.png" alt="Zektor PROAUDIO16 - connections - output 02" width="230" height="">
</a>

* **Analog Output (01-16):** L/R audio output.

* **Coax Output (01-16):** Digital coaxial output.
