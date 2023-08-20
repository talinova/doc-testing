---
title: "Serial AMX Precis DSP Driver"
tags: creator, driver, equipment, harman, amx, precis
date:
  created: "05/09/2022"
  modified: "12/12/2022"
description: Serial (RS232) driver for the Harman AMX Precis DSP Stereo RCA DVC.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/amx-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/amx-logo.png" alt="BSS harman Logo" width="700" height="" class="center">
</a>
</div>

# Serial AMX Precis DSP Driver

This driver supports the [Harman AMX Precis DSP](https://www.amx.com/en/products/precis-dsp-stereo-rca-dvc "Harman AMX Precis DSP") through serial connection.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-serial-amx-precis-dsp.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-serial-amx-precis-dsp.png" alt="Harman AMX Precis DSP serial configuration" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">


* **Baud Rate:** Set to 300 by default.

* **Flow Control:** Sets the serial port handshake type.
  * None - Turned off.
  * Hardware - Hardware flow control.
  * XON/XOFF - Software flow control.
  * Unknown - Flow control is unknown.

* **Parity:** Sets the serial port parity type for error detecting.
  * None - Turned off.
  * Even - Even parity bit.
  * Odd - Odd parity bit.
  * Unknown - Parity is unknown.

* **Data Bits:** Set to 8.

* **Stop Bits:** Set to either 1 or 2.

* **Level Number:** This Corresponds to the Virtual Matrix number. This is usually 0.


### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-serial-amx-precis-dsp-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-serial-amx-precis-dsp-connections-input.png" alt="Harman AMX Precis DSP serial - connections input" width="300" height="">
</a>

* **Input (01-18):** Up to eighteen L/R audio inputs.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/harman-serial-amx-precis-dsp-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/harman-serial-amx-precis-dsp-connections-output.png" alt="Harman AMX Precis DSP serial - connections output" width="300" height="">
</a>

* **Output (01-18):** Up to eighteen L/R audio outputs.
