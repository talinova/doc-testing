---
title: "AVPro Edge AC-MXNET-CBOX Switch Driver"
tags: creator, driver, equipment, avpro, mxnet, cbox
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: IP driver for the AVPro Edge MXNet Control Box.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/avpro-edge-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/avpro-edge-logo.png" alt="AVPro Edge Logo" width="700" height="" class="center">
</a>
</div>

# AVPro Edge AC-MXNET-CBOX Switch Driver
This AVPro Edge driver interfaces with the [CBOX switch](https://www.avproedge.com/ac-mxnet-cbox.html) device, which in turn controls multi-cast switches, receivers, and transmitters. 

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-01.png" alt="SAVI Creator AVPro Edge AC-MXNET-CBOX configuration" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-02.png" alt="SAVI Creator AVPro Edge AC-MXNET-CBOX configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **TX(01-24) ID:** Transmitter port ID.

* **RX(01-24) ID:** Receiver port ID.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-connections-input.png" alt="SAVI Creator AVPro Edge AC-MXNET-CBOX input connections upper" width="300" height="">
</a>


* **TX(01-24):** Connects to up to 24 individual source transmitters.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/avpro-edge-ac-mxnet-cbox-switch-connections-output.png" alt="SAVI Creator AVPro Edge AC-MXNET-CBOX output connections upper" width="300" height="">
</a>


* **RX(01-24):** Connects to up to 24 individual output receivers.