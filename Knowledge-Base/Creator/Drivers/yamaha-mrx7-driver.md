---
title: "Yamaha MRX7 Component Driver"
tags: creator, driver, equipment, yamaha, mrx
date:
  created: "05/13/2022"
  modified: "12/12/2022"
description: Resource for the Yamaha MRX7 device driver.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/yamaha-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/yamaha-logo.png" alt="Yamaha Logo" width="700" height="">
</a>
</div>

# Yamaha MRX7 Component Driver
This driver has limited control over faders, matrix mixers, routers, and source selectors in the [MRX7](https://usa.yamaha.com/products/proaudio/processors/mrx7-d/index.html) setup. Configure the components separately in the **MTX-MRX Editor** and download the "Remote Control List." This list can be uploaded to the SAVI Admin page by selecting the "Import MRX7 CSV File" option. 

One of these drivers will need to be used for each different component of the MRX7 project. 


#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/yamaha-mrx7-component.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/yamaha-mrx7-component.png" alt="Yamaha MRX7 Component configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Unit ID:** Set to 1 by default.

* **Component ID:** Set to 20000 by default.

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Volume Scale:** Sets the volume indicators to either dB or Percent.


### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/yamaha-mrx7-component-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/yamaha-mrx7-component-connections-input.png" alt="Yamaha MRX7 Component input connections" width="230" height="">
</a>

* **Input (01-32):** Up to thirty-two audio inputs.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/yamaha-mrx7-component-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/yamaha-mrx7-component-connections-output.png" alt="Yamaha MRX7 Component output connections" width="230" height="">
</a>


* **Output (01-32):** Up to thirty-two audio outputs.
