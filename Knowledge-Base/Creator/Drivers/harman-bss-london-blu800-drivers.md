---
title: "Harman BSS London Blu-800 Drivers"
tags: creator, driver, equipment, harman, bss, blu, london
date:
  created: "05/09/2022"
  modified: "11/01/2022"
description: Resource for the BSS London BLU-800 signal processor.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/bss-harman-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/bss-harman-logo.png" alt="BSS harman Logo" width="700" height="" class="center">
</a>
</div>

# Harman BSS London Blu-800 Drivers

These drivers support the [Harman BSS BLU-800 Matrix](https://bssaudio.com/en/products/blu-800 "Harman DBX Zone Pro 1260 Matrix"), [Harman BSS BLU-806 Matrix](https://bssaudio.com/en/products/blu-806da-blu-806), and the [Harman BSS BLU-160 Matrix](https://bssaudio.com/en/products/blu-160) through the Audio Architect software. 

Gain modules are needed for volume control and one of the Source or Matrix drivers are needed for source control within SAVI. Requirements are determined by the virtual project setup within the Audio Architect software.

## Gain Module
This driver controls volume only. It connects on a one-to-one (input to output) basis so a driver will be needed for each input and output pair. Connections should never be used, rather use this driver as an Alternate Volume Control through your project's output device card.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-gain-module.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-gain-module.png" alt="Harman BSS London Blu-800 Gain Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **HiQnet Address:** A 14 digit address key (such as `0x083203000100`).

* **Throttle Time (ms):** This device may have issues processing too many commands at once. This value will set how many milliseconds to wait after each command to the unit. Set to 0 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-gain-module-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-gain-module-connections-input.png" alt="Harman BSS London Blu-800 Gain Module - connections input" width="300" height="">
</a>

* **Input 01:** Euroblock (phoenix) connector.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-gain-module-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-gain-module-connections-output.png" alt="Harman BSS London Blu-800 Gain Module - connections output" width="300" height="">
</a>

* **Output 01:** Euroblock (phoenix) connector.

<!--
## N Input Gain Module
This driver controls volume only. Connections are not needed when using this driver as an Alternate Volume Control.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-n-input-gain-module.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-n-input-gain-module.png" alt="Harman BSS London Blu-800 N Input Gain Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **HiQnet Address:** A 14 digit address key (such as `0x083203000100`).

* **Throttle Time (ms):** This device may have issues processing too many commands at once. This value will set how many milliseconds to wait after each command to the unit. Set to 0 by default.

### Connections

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-n-input-gain-module-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-n-input-gain-module-connections-output.png" alt="Harman BSS London Blu-800 N Input Gain Module - connections output" width="300" height="">
</a>

* **Output (01-11):** Euroblock (phoenix) connectors.


-->
----



## Matrix Mixer Module
This driver will require Gain Modules to control volume.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-mixer-module.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-mixer-module.png" alt="Harman BSS London Blu-800 Matrix Mixer Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **HiQnet Address:** A 14 digit address key (such as `0x083203000100`).

* **Throttle Time (ms):** This device may have issues processing too many commands at once. This value will set how many milliseconds to wait after each command to the unit. Set to 0 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-mixer-module-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-mixer-module-connections-input.png" alt="Harman BSS London Blu-800 Matrix Mixer Module - connections input" width="300" height="">
</a>

* **Input (01-48):** Euroblock (phoenix) connectors.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-mixer-module-connections-output.png.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-mixer-module-connections-output.png" alt="Harman BSS London Blu-800 Matrix Mixer Module - connections output" width="300" height="">
</a>

* **Output (01-48):** Euroblock (phoenix) connectors.


## Matrix Router Module
This driver will require Gain Modules to control volume.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-router-module.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-router-module.png" alt="Harman BSS London Blu-800 Matrix Router Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **HiQnet Address:** A 14 digit address key (such as` 0x083203000100`).

* **Throttle Time (ms):** This device may have issues processing too many commands at once. This value will set how many milliseconds to wait after each command to the unit. Set to 0 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-router-module-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-router-module-connections-input.png" alt="Harman BSS London Blu-800 Matrix Router Module - connections input" width="300" height="">
</a>

* **Input (01-48):** Euroblock (phoenix) connectors.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-router-module-connections-output.png.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-matrix-router-module-connections-output.png" alt="Harman BSS London Blu-800 Matrix Router Module - connections output" width="300" height="">
</a>

* **Output (01-48):** Euroblock (phoenix) connectors.




## Source Matrix Module
This driver will require Gain Modules to control volume.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-matrix-module.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-matrix-module.png" alt="Harman BSS London Blu-800 Source Matrix Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **HiQnet Address:** A 14 digit address key (such as `0x083203000100`).

* **Throttle Time (ms):** This device may have issues processing too many commands at once. This value will set how many milliseconds to wait after each command to the unit. Set to 0 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-matrix-module-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-matrix-module-connections-input.png" alt="Harman BSS London Blu-800 Source Matrix Module - connections input" width="300" height="">
</a>

* **Input (01-48):** Euroblock (phoenix) connectors.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-matrix-module-connections-output.png.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-matrix-module-connections-output.png" alt="Harman BSS London Blu-800 Source Matrix Module - connections output" width="300" height="">
</a>

* **Output (01-48):** Euroblock (phoenix) connectors.


## Source Selector Module
This driver will require Gain Modules to control volume.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-selector-module.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-selector-module.png" alt="Harman BSS London Blu-800 Source Selector Module" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **HiQnet Address:** A 14 digit address key (such as `0x083203000100`).

* **Throttle Time (ms):** This device may have issues processing too many commands at once. This value will set how many milliseconds to wait after each command to the unit. Set to 0 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-selector-module-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-selector-module-connections-input.png" alt="Harman BSS London Blu-800 Source Selector Module - connections input" width="300" height="">
</a>

* **Input (01-48):** Euroblock (phoenix) connectors.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-selector-module-connections-output.png.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-bss-london-blu-800-source-selector-module-connections-output.png" alt="Harman BSS London Blu-800 Source Selector Module - connections output" width="300" height="">
</a>

* **Output 01:** Euroblock (phoenix) connectors.
