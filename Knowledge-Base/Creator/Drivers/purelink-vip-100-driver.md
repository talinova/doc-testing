---
title: "Purelink VIP-100 II RX Driver"
tags: creator, driver, equipment, purelink, vip-100-ii
date:
  created: "09/16/2022"
  modified: "12/12/2022"
description: Resource for the Purelink VIP-100 II.
---

<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/purelink-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/purelink-logo.png" alt="Purelink Logo" width="" height="">
</a>
</div>

# Purelink VIP-100 II RX Driver

<!--
Future: include what controls the transmitters.
-->

This driver controls the [receiver](https://www.purelinkav.com/product/hdmi-over-ip-receiver-decoder-with-poe/) which must be configured to connect to Transmitters. Each transmitter is connected to a channel source and each receiver connects to the back of a display to allow switching between all available transmitters.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/purelink-vip-100-ii-rx.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/purelink-vip-100-ii-rx.png" alt="Purelink VIP-100 II RX" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/purelink-vip-100-ii-rx-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/purelink-vip-100-ii-rx-connections-input.png" alt="Purelink VIP-100 II RX - input" width="300" height="">
</a>


* **Channel (00-63):** Up to sixty-four HDMI transmitters. Each transmitter should already be connected and configured.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/purelink-vip-100-ii-rx-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/purelink-vip-100-ii-rx-connections-output.png" alt="Purelink VIP-100 II RX - output" width="300" height="">
</a>

* **Output 01:** The HDMI output on the back of the receiver.
