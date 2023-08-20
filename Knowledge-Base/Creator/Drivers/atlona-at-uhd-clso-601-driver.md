---
title: "Atlona AT-UHD-CLSO-601 Driver"
tags: creator, driver, equipment, atlona, clso, video, matrix
date:
  created: "03/25/2022"
  modified: "12/07/2022"
description: IP driver for the Atlona AT-UHD-CLSO-601 4K/UHD Six-Input Multi-Format Switcher.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/atlona-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/atlona-logo.png" alt="Atlona Logo" width="700" height="" class="center">
</a>
</div>

# Atlona AT-UHD-CLSO-601 Driver
This driver interfaces with this specific [Atlona video matrix](https://atlona.com/product/at-uhd-clso-601/ "Atlona video matrix"). Specifications on the matrix itself can be found on the Atlona site.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-at-uhd-clso-601.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-at-uhd-clso-601.png" alt="Atlona AT UHD CLSO 601 configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Port:** The IP address port that the device is open to. Set to 23 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-at-uhd-clso-601-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-at-uhd-clso-601-connections-input.png" alt="Atlona AT UHD CLSO 601 - input connections upper" width="300" height="">
</a>

* **HDMI (1-4):** Corresponds to the four HDMI inputs on the back of the device. Can pair with audio input from matching labeled 3-pos euroblock audio inputs.

* **VGA (1-2):** Corresponds to the two VGA inputs on the back of the device (15pin blue connectors). Used for SD computer displays. Pairs with audio input from matching RS232 or L/R audio 3-pos euroblock audio inputs.

* **SVIDEO (1-2):** Corresponds to the two VGA inputs on the back of the device (15pin blue connectors). Compatible with S-Video signals. Pairs with audio input from matching RS232 or L/R audio 3-pos euroblock audio inputs.

* **CVBS (1-2):** Corresponds to the two VGA inputs on the back of the device (15pin blue connectors). Compatible with composite signals. Pairs with audio input from matching RS232 or L/R audio 3-pos euroblock audio inputs.

* **COMP (1-2):** Corresponds to the two VGA inputs on the back of the device (15pin blue connectors). Compatible with component signals. Pairs with audio input from matching RS232 or L/R audio 3-pos euroblock audio inputs.

* **LINE IN:** 3-pos euroblock audio input used for plain Line-in or MIC input.
>***Be sure to select MIC (self-powered), 48V (supplies 48V to MIC), or LINE (balanced, unbalanced, mono, or two channel) for the appropriate audio source.***

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-at-uhd-clso-601-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-at-uhd-clso-601-connections-output.png" alt="Atlona AT UHD CLSO 601 - output connections" width="300" height="">
</a>

* **LINE OUT:** RJ45 output for use with AT-UHD-EX-100CE-RX HDBaseT device.

* **Room Selection:** A deprecated output. Not recommended for use.

* **HDMI Out:** Corresponds to the HDMI output on the back of the device.
