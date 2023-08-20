---
title: "QSC Q-SYS Drivers"
tags: creator, driver, equipment, qsc, q-sys
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: Resource for the QSC drivers which work together to control different QSC devices.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/qsc-audio-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/qsc-audio-logo.png" alt="QSC Logo" width="700" height="">
</a>
</div>

# QSC Q-SYS Drivers

Control for [Q-SYS products](https://www.qsys.com/products-solutions/) is separated into these two drivers; A volume level driver and a source routing driver.

### Level Driver
A Level driver is needed for every output you wish to control. When using the Router Driver as well, these level drivers must be set as the Alternate Volume Control in the Audio Zone. This driver can be used with other router drivers and still set as the Alternate Volume Control.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-level.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-level.png" alt="QSC QSYS Level" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Username used to connect to the QSys Core. Leave blank if no login is used.

* **PIN:** PIN used to connect to the QSys Core. Leave blank if no login is used.

* **Max Gain:** Maximum amount of gain allowed. Set to 20 by default.

* **Min Gain:** Minimum amount of gain allowed. Set to 20 by default.

* **Gain Control Name:** What to name the gain control. This needs to match the named controls found in the Q-SYS Core system.

* **Mute Control Name:** What to name the mute control. This needs to match the named controls found in the Q-SYS Core system.

### Connections
If using this driver as an Alternate Volume Control, leave all connections blank.

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-level-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-level-connections-input.png" alt="QSC Q-SYS Level - connections - input" width="300" height="">
</a>

* **Input:** Connect to the output on the Router Driver you wish to control.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-level-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-level-connections-output.png" alt="QSC Q-SYS Level - connections - output" width="300" height="">
</a>

* **Output:** Connect to an audio zone.




## Router Driver
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-01.png" alt="QSC Q-SYS Router 01" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-02.png" alt="QSC Q-SYS Router 02" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Username used to connect to the QSys Core. Leave blank if no login is used.

* **PIN:** PIN used to connect to the QSys Core. Leave blank if no login is used.

* **Output Control Name (1-32)** What name to use for each output control. This needs to match the named controls found in the Q-SYS Core system.

* **Output Mute Control Name (1-32)** What name to use for each output mute control. This needs to match the named controls found in the Q-SYS Core system.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-connections-input.png" alt="QSC Q-SYS Router - connections input" width="300" height="">
</a>


* **Input (1-32):** Up to thirty-two inputs.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-router-connections-output.png" alt="QSC Q-SYS Router - connections output" width="300" height="">
</a>


* **Output (1-32):** Up to thirty-two outputs.


----


## Media Stream Receiver
This driver allows changing the stream URL value.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-media-stream-receiver.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-media-stream-receiver.png" alt="QSC Q-SYS Media Stream Receiver" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Username used to connect to the QSys Core. Leave blank if no login is used.

* **PIN:** PIN used to connect to the QSys Core. Leave blank if no login is used.

* **URL Control Name:** What name to use for the URL control. This needs to match the named controls found in the Q-SYS Core system.

* **Channel (1-2) Gain Control Name:** What name to use for each gain control. This needs to match the named controls found in the Q-SYS Core system.

* **Channel (1-2) Mute Control Name:** What name to use for each mute control. This needs to match the named controls found in the Q-SYS Core system.

* **Enable Control Name:** What name to use for the enable control toggle setting. This needs to match the named controls found in the Q-SYS Core system.

### Connections

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-media-stream-receiver-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-media-stream-receiver-connections-output.png" alt="QSC Q-SYS Media Stream Receiver - connections output" width="300" height="">
</a>

* **Channel (1-2):** These are the two audio channels on the output in the QSC project. If the stream is mono, then both outputs will be the same. If the stream is stereo, then channels will be right and left.

----

## Snapshot
This driver allows reverting to a specific setting configuration in the Q-SYS Core system.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-snapshot.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/qsc-qsys-snapshot.png" alt="QSC QSYS Snapshot" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Username used to connect to the QSys Core. Leave blank if no login is used.

* **PIN:** PIN used to connect to the QSys Core. Leave blank if no login is used.
